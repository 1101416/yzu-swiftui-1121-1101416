<h1>HW1</h1>
```swift
import SwiftUI

struct ContentView: View {
    var body: some View {
        Text("1101416 李柏翰")
            .fontWeight(.bold)
            .font(.title)
            .fontWeight(.heavy)
        Image(systemName: "trash")
            .symbolRenderingMode(.multicolor)
        
        Image("影像內容")
            .resizable()
            .scaledToFit()
            .aspectRatio(/*@START_MENU_TOKEN@*/1.5/*@END_MENU_TOKEN@*/, contentMode: /*@START_MENU_TOKEN@*/.fill/*@END_MENU_TOKEN@*/)
            .overlay(
                Text("Hi! I am Bryan, I am happy to let you see my self-photo that I was 16 years old!!")
                    .foregroundColor(.white)
                    .frame(width: 350, height: /*@START_MENU_TOKEN@*/100/*@END_MENU_TOKEN@*/, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
                    .opacity(0.8)
                    .lineSpacing(20)
                    .fontWeight(.heavy)
                    .background(Color.gray)
                    .cornerRadius(10),alignment: .bottom
            )    
    }
}
```
<img width="40%"  src="https://raw.githubusercontent.com/ncudemo/yzu-swiftui-1121-864106/main/S__3563523.jpg">
