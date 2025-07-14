

- Network Extension
- NEFilterPacketProvider
-  handler 

Instance Property

# handler

macOS 15.0+

``` source
var handler: ((NEFilterPacketContext, NWInterface, NETrafficDirection, UnsafeRawBufferPointer) -> NEFilterPacketProvider.Verdict)? { get set }
```

