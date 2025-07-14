

- Security Interface
- SFAuthorizationPluginView
-  callbacks() 

Instance Method

# callbacks()

Returns the authorization callbacks structure with which this instance was initialized.

macOS 10.5+

``` source
func callbacks() -> UnsafePointer!
```

## Return Value

An object of type AuthorizationCallbacks.

## Discussion

Use the AuthorizationCallbacks structure to get the function pointers to functions such as `SetResult` and `SetContextValue`.

## See Also

### Getting Instance Information

func engineRef() -> AuthorizationEngineRef!

Returns the authorization engine handle with which this instance was initialized.

func lastError() -> (any Error)!

Returns the last error that occurred during evaluation.

