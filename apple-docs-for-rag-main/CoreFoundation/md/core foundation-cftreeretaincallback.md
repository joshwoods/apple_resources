

- Core Foundation
-  CFTreeRetainCallBack 

Type Alias

# CFTreeRetainCallBack

Callback function used to retain a program-defined information pointer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFTreeRetainCallBack = (UnsafeRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`info`  

The program-supplied information pointer provided in a CFTreeContext structure.

## Return Value

The value to use whenever the information pointer is retained, which is usually the `info` parameter passed to this callback, but may be a different value if a different value should be used.

## See Also

### Callbacks

typealias CFTreeApplierFunction

Type of the callback function used by the CFTree apply function.

typealias CFTreeCopyDescriptionCallBack

Callback function used to provide a description of the program-defined information pointer.

typealias CFTreeReleaseCallBack

Callback function used to release a previously retained program-defined information pointer.

