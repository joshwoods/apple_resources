

- Security Interface
- SFAuthorizationPluginView
-  engineRef() 

Instance Method

# engineRef()

Returns the authorization engine handle with which this instance was initialized.

macOS 10.5+

``` source
func engineRef() -> AuthorizationEngineRef!
```

## Return Value

A handle of type AuthorizationEngineRef.

## Discussion

Use the authorization engine handle when you call the functions in the AuthorizationCallbacks structure to set a result or a context value.

## See Also

### Getting Instance Information

func callbacks() -> UnsafePointer&lt;AuthorizationCallbacks>!

Returns the authorization callbacks structure with which this instance was initialized.

func lastError() -> (any Error)!

Returns the last error that occurred during evaluation.

