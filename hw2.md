<h1>HW2</h1>

  ```swift

      import SwiftUI

struct ContentView: View {
    @State private var playerSign: Sign?
    @State private var computerSign: Sign?
    @State private var gameResult: String?
    
    enum Sign: String {
        case rock
        case paper
        case scissors
        
        var emoji: String {
            switch self {
            case .rock:
                return "✊"
            case .paper:
                return "✋"
            case .scissors:
                return "✌️"
            }
        }
        
        func gamestate(against opponentSign: Sign) -> String {
            if self == opponentSign {
                return "It's a draw!"
            }
            if (self == .rock && opponentSign == .scissors) ||
                (self == .paper && opponentSign == .rock) ||
                (self == .scissors && opponentSign == .paper) {
                return "You win!"
            } else {
                return "You lose!"
            }
        }
    }
    
    var body: some View {
        VStack {
            if playerSign == nil {
                Text("Choose a sign:")
                    .padding(.bottom, 10)
                    .font(.system(size:30))
                HStack {
                    Button(action: {
                        playGame(.rock)
                    }) {
                        Text(Sign.rock.emoji)
                            .font(.largeTitle)
                    }
                    Button(action: {
                        playGame(.paper)
                    }) {
                        Text(Sign.paper.emoji)
                            .font(.largeTitle)
                    }
                    Button(action: {
                        playGame(.scissors)
                    }) {
                        Text(Sign.scissors.emoji)
                            .font(.largeTitle)
                    }
                }
            } else {
                Text("You chose: \(playerSign!.emoji)")
                    .padding(.bottom, 10)
                    .font(.system(size:30))
                if let computerSign = computerSign {
                    Text("Computer chose: \(computerSign.emoji)")
                        .padding(.bottom, 10)
                        .font(.system(size:30))
                }
                if let gameResult = gameResult {
                    Text(gameResult)
                        .font(.title)
                        .font(.system(size:30))
                }
                Button(action: {
                    restartGame()
                }) {
                    Text("Play Again")
                        .padding(.all, 10)
                        .font(.system(size:30))
                }
            }
        }
    }
    
    func playGame(_ chosenSign: Sign) {
        playerSign = chosenSign
        computerSign = randomSign()
        gameResult = playerSign!.gamestate(against: computerSign!)
    }
    
    func randomSign() -> Sign {
        let randomIndex = Int.random(in: 0...2)
        if randomIndex == 0 {
            return .rock
        } else if randomIndex == 1 {
            return .paper
        } else {
            return .scissors
        }
    }
    
    func restartGame() {
        playerSign = nil
        computerSign = nil
        gameResult = nil
    }
}

    
  ```
  <iframe style="width:560px; height:315px;" src="https://raw.githubusercontent.com/1101416/yzu-swiftui-1121-1101416/main/hw2.mp4" frameborder="0" allowfullscreen></iframe>
