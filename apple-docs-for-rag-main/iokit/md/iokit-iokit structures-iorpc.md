

- IOKit
- IOKit Structures
-  IORPC 

Structure

# IORPC

Mac Catalyst 13.0+macOS 10.15+

``` source
struct IORPC
```

## Topics

### Initializers

init()

init(message: UnsafeMutablePointer&lt;IORPCMessageMach>!, reply: UnsafeMutablePointer&lt;IORPCMessageMach>!, sendSize: UInt32, replySize: UInt32)

### Instance Properties

var message: UnsafeMutablePointer&lt;IORPCMessageMach>!

var reply: UnsafeMutablePointer&lt;IORPCMessageMach>!

var replySize: UInt32

var sendSize: UInt32

