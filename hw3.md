<h1>HW3</h1>
    
```swift

      import SwiftUI
struct ContentView: View {
    var body: some View{
        VStack{
            TitleView()
            ZStack{
                FoodView()
                    .offset(x:-100)
                Text("在衣櫃裡面翻到的地呱球")
                    .foregroundColor(.black)
                    .offset(x:50,y:0)
            }.frame(minWidth: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealWidth: /*@START_MENU_TOKEN@*/100/*@END_MENU_TOKEN@*/, maxWidth: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, minHeight: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealHeight: 200, maxHeight: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
                .background(Color(.yellow))
            HStack{
                clothview()
                clothview1()
                clothview2()
            }.frame(minWidth: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealWidth: /*@START_MENU_TOKEN@*/100/*@END_MENU_TOKEN@*/, maxWidth: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, minHeight: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealHeight: 200, maxHeight: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
                .background(Color(.brown))
            HStack{
                clothview3()
                Text("去馬來西亞買的")
                    .font(.system(size:10))
                    .foregroundColor(.black)
                    .opacity(/*@START_MENU_TOKEN@*/0.8/*@END_MENU_TOKEN@*/)
                    .background(Color.yellow)
                    .offset(x:-95,y:-20)
                clothview4()
            }.frame(minWidth: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealWidth: /*@START_MENU_TOKEN@*/100/*@END_MENU_TOKEN@*/, maxWidth: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, minHeight: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealHeight: 200, maxHeight: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
                .background(Color(.systemBrown))
            HStack{
                clothview5()
                clothview6()
            }.frame(minWidth: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealWidth: /*@START_MENU_TOKEN@*/100/*@END_MENU_TOKEN@*/, maxWidth: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, minHeight: /*@START_MENU_TOKEN@*/0/*@END_MENU_TOKEN@*/, idealHeight: 200, maxHeight: /*@START_MENU_TOKEN@*/.infinity/*@END_MENU_TOKEN@*/, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
                .background(Color(.lightGray))
        }
    }
}

struct TitleView: View {
    var body: some View {
        VStack(alignment: .center, spacing: 2){
            Text("Bryan空空的")
                .font(.system(size: 30))
            Text("衣櫃")
                .font(.title)
                .foregroundColor(.brown)
        }
    }
}
struct FoodView: View {
    var body: some View {
        VStack{
            Image("地呱球")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
        }
    }
}
struct clothview: View {
    var body: some View {
        VStack{
            Image("影像內容")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("黑色上衣")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}
struct clothview1: View {
    var body: some View {
        VStack{
            Image("影像內容 1")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("綠色上衣")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}
struct clothview2: View {
    var body: some View {
        VStack{
            Image("影像內容 2")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("燈心絨上衣")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}

struct clothview3: View {
    var body: some View {
        VStack{
            Image("影像內容 3")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("燈心絨短褲")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}
struct clothview4: View {
    var body: some View {
        VStack{
            Image("影像內容 4")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("寬鬆短褲")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}
struct clothview5: View {
    var body: some View {
        VStack{
            Image("影像內容 5")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("火焰長襪")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}
struct clothview6: View {
    var body: some View {
        VStack{
            Image("影像內容 6")
                .resizable()
                .aspectRatio(contentMode:.fit)
                .frame(width: 100, alignment: /*@START_MENU_TOKEN@*/.center/*@END_MENU_TOKEN@*/)
            Text("Nike長襪")
                .fontWeight(.bold)
                .font(.system(size:20))
        }
    }
}


    
```
<img width="40%"  src="https://raw.githubusercontent.com/1101416/yzu-swiftui-1121-1101416/main/hw3.jpg">
