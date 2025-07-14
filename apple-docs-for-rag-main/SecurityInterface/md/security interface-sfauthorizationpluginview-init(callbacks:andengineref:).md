

- Security Interface
- SFAuthorizationPluginView
-  init(callbacks:andEngineRef:) 

Initializer

# init(callbacks:andEngineRef:)

Initializes a new authorization plug-in view with the specified callbacks and authorization engine handle.

macOS 10.5+

``` source
init!(
    callbacks: UnsafePointer!,
    andEngineRef engineRef: AuthorizationEngineRef!
)
```

## Parameters 

`callbacks`  

The structure of type AuthorizationCallbacks provided to the authorization plug-in in its AuthorizationPluginCreate function.

`engineRef`  

The handle of type AuthorizationEngineRef provided to the authorization plug-in in its MechanismCreate function.

## Return Value

An initialized `SFAuthorizationPluginView` instance.

## See Also

### Related Documentation

Authorization Services Programming Guide

