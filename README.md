```swift
include WorkKit
include FunKit

class AdeLife(){
  public var bDate : "22.06.1976"
  public var age : TimeInterval!
  public var fun = ["reading","learning","playing piano","bike","coding","travel"]
  public var workCompanies = ["Ubisoft","Gameloft"]
  public var knowledge = ["SWIFT","C++","GIT","JIRA","SVN","3DSMAX","Blender","Photoshop","many many other"]
  public var languages = ["English=fluent","German=beginner","Romanian=native","Russian=fluent"]
  public var email = "oposum2012@gmail.com" 
  
  private var endDate : Date!
  
  init(_ e:Date){
    self.endDate = e
    life()
  }
  
  private func life(){
    while Date.curentDate < endDate {
      switch Date.dayOfTheWeek(){
      case workDay:
        var task = CurentCompany.Tasks.curentTask()
        getTaskDone(task)
        if time < sleepTime { funWithFalimy() }
      default:
         if agenda() == .travel { funWithFalimy(.travel); trave+=1 }
         if agenda() == .ski { ski(slope.hardcore < 100% ? true:false); }
      }
    }
  }
  
  private func funWithFalimy(_ t:Int=0){
    var currentFun = t > 0 ? t:rnd(fun.count)
    doTheFan(fan[currentFun])
  }
  
  public func interaction(_ d:Date,_ length:TimeInterval){
    age = TimeInterval(d - bDate)
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
  
  public func ski(_ b:Bool){
    print("https://youtu.be/CXrAzc2wayk", b ? " was fun!":" was even better!")
  }
}

```
