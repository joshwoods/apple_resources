

- Core Foundation
-  CFTreeApplierFunction 

Type Alias

# CFTreeApplierFunction

Type of the callback function used by the CFTree apply function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFTreeApplierFunction = (UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`value`  

The current child of a tree that is being iterated.

`context`  

The program-defined context parameter that was passed to the applier function.

## Discussion

This callback is used by the CFTreeApplyFunctionToChildren(_:_:_:) applier function.

## See Also

### Callbacks

typealias CFTreeCopyDescriptionCallBack

Callback function used to provide a description of the program-defined information pointer.

typealias CFTreeReleaseCallBack

Callback function used to release a previously retained program-defined information pointer.

typealias CFTreeRetainCallBack

Callback function used to retain a program-defined information pointer.

