

- IOKit
- IOKit Structures
-  IORPCMessage 

Structure

# IORPCMessage

Mac Catalyst 13.0+macOS 10.15+

``` source
struct IORPCMessage
```

## Topics

### Initializers

init()

init(msgid: UInt64, flags: UInt64, objectRefs: UInt64, objects: ())

### Instance Properties

var flags: UInt64

var msgid: UInt64

var objectRefs: UInt64

var objects: ()

