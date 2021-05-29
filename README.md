```swift
include WorkKit
include FunKit

class AdeLife(){
  public var bDate : "22.06.1976"
  public var fun = ["reading","learning","playing piano","bike","coding","travel"]
  
  private var age : Date!
  private var endDate : Date!
  
  init(_ e:Date){
    self.endDate = e
    life()
  }
  
  public func interaction(_ d:Date,_ length:TimeInterval){
    age = d - bDate
    var interationTime = 0
    while interactionTime < length {
      talkNice()
      listenCarrefully()
      learn()
      share()
      haveFun()
      interactionTime+=1
    }
  }
  
  private func life(){
    while Date.curentDate < endDate {
      switch Date.dayOfTheWeek(){
      case workDay:
        var task = Tasks.curentTask()
        getTaskDone()
        if time < sleepTime { funWithFalimy() }
      default:
         if agenda() == .travel { funWithFalimy(.travel); trave+=1 }
         if agenda() == .ski { ski(tired < 10000% ? true:true); }
      }
    }
  }
  
  private func funWithFalimy(_ t:Int=0){
    var currentFun = t > 0 ? t:rnd(fun.count)
    doTheFan(fan[currentFun])
  }
  
  private func ski(_ b:Bool){
    print("https://youtu.be/CXrAzc2wayk")
  }
}

```
