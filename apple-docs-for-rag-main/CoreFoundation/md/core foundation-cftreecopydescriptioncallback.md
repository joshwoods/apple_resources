

- Core Foundation
-  CFTreeCopyDescriptionCallBack 

Type Alias

# CFTreeCopyDescriptionCallBack

Callback function used to provide a description of the program-defined information pointer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFTreeCopyDescriptionCallBack = (UnsafeRawPointer?) -> Unmanaged?
```

## Parameters 

`info`  

The program-supplied information pointer provided in a CFTreeContext structure.

## Return Value

A textual description of `info`. The caller is responsible for releasing this object.

## See Also

### Callbacks

typealias CFTreeApplierFunction

Type of the callback function used by the CFTree apply function.

typealias CFTreeReleaseCallBack

Callback function used to release a previously retained program-defined information pointer.

typealias CFTreeRetainCallBack

Callback function used to retain a program-defined information pointer.

