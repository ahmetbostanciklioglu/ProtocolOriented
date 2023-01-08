# ProtocolOriented
Protocol Oriented Programming (POP)



**Protocol Oriented:**
```
protocol ProtocolOriented {
    var protocolProperty: String { get set } // get -> read; set -> write
    func protocolFunction()
    mutating func mutatingProtocolFunction(param: String)
}

extension ProtocolOriented {
    func protocolFunction() {
        print("\(protocolProperty)")
    }
}

struct protocolOrientedStruct : ProtocolOriented{
    var protocolProperty: String

    mutating func mutatingProtocolFunction(param: String) {
        print("mutating protocol function")
    }
}


var protocolObject = protocolOrientedStruct(protocolProperty: "Ahmet")

protocolObject.protocolFunction() 
protocolObject.mutatingProtocolFunction(param: "Alli")
```
