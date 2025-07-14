

- Authentication Services
- ASWebAuthenticationSession
-  cancel() 

Instance Method

# cancel()

Cancels a web authentication session.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.15+visionOS 1.0+watchOS 6.2+

``` source
func cancel()
```

## Mentioned in 

Authenticating a User Through a Web Service

## Discussion

If the session has already presented a view with the authentication webpage, calling this method dismisses that view. Calling cancel() on an already canceled session has no effect.

## See Also

### Starting and Stopping a Session

var canStart: Bool

A Boolean indicating whether the session can begin.

func start() -> Bool

Starts a web authentication session.

