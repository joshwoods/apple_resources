

- ARKit
- ARSessionObserver
-  session(\_:didFailWithError:) 

Instance Method

# session(\_:didFailWithError:)

Tells the delegate that the session has stopped running due to an error.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didFailWithError error: any Error
)
```

## Parameters 

`session`  

The session providing information.

`error`  

An object describing the failure.

## See Also

### Handling Errors

let ARErrorDomain: String

The domain for error objects produced by an AR session.

