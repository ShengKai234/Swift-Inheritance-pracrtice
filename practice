# Swift-Inheritance-pracrtice

class Transportation {
    var speed = 0
    var information :String{
        return "的時速為:\(speed)km/h"
    }
    func distance(hour a:Int) -> Int{
        return speed * a
    }
}
let some = Transportation()
some.speed = 10
print("這個交通工具\(some.information)")

class Car:Transportation{
    var wheel = 4
}
let tricycle = Car()
tricycle.speed = 1
tricycle.wheel = 3
print("三輪車\(tricycle.information)，輪子有\(tricycle.wheel)")

class ElectricCar:Car{
    var energe = "電力"
}
let electricCar = ElectricCar()
electricCar.speed = 20
print("這台電動車是靠\(electricCar.energe)發動的，輪子有\(electricCar.wheel)，它\(electricCar.speed)")

class broken:Transportation{
    override func distance(hour a: Int) -> Int {
        print("這台車無法行駛，速度為\(speed)")
        return speed * a
    }
}
let brokenCar = broken()
brokenCar.distance(hour: 100)

class Stuck:Transportation{
    override var information: String{
        return "現在阻塞了"
    }
}
let traffic = Stuck()
print(traffic.information)
