

- IOBluetooth
- OBEXSessionEvent
-  init(type:session:refCon:isEndOfEventData:reserved1:reserved2:u:) 

Initializer

# init(type:session:refCon:isEndOfEventData:reserved1:reserved2:u:)

macOS

``` source
init(
    type: OBEXSessionEventType,
    session: OBEXSessionRef!,
    refCon: UnsafeMutableRawPointer!,
    isEndOfEventData: DarwinBoolean,
    reserved1: UnsafeMutableRawPointer!,
    reserved2: UnsafeMutableRawPointer!,
    u: OBEXSessionEvent.__Unnamed_union_u
)
```

