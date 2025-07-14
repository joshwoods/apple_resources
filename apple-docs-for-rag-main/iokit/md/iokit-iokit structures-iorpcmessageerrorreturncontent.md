

- IOKit
- IOKit Structures
-  IORPCMessageErrorReturnContent 

Structure

# IORPCMessageErrorReturnContent

Mac Catalyst 13.0+macOS 10.15+

``` source
struct IORPCMessageErrorReturnContent
```

## Topics

### Initializers

init()

init(hdr: IORPCMessage, result: kern_return_t, pad: UInt32)

### Instance Properties

var hdr: IORPCMessage

var pad: UInt32

var result: kern_return_t

