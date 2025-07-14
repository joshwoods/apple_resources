

- Objective-C Runtime
- NSObject
-  authorizationViewReleasedAuthorization(\_:) 

Instance Method

# authorizationViewReleasedAuthorization(\_:)

Sent to the delegate to indicate that deauthorization is about to occur.

macOS 10.3+

``` source
func authorizationViewReleasedAuthorization(_ view: SFAuthorizationView!)
```

## Discussion

This method is called after deauthorization has been approved (either you called the deauthorize(_:) method, or the user clicked an open lock icon and the authorizationViewShouldDeauthorize(_:) delegate method did not cancel the operation), and before the user is deauthorized (that is, before the authorizationViewDidDeauthorize(_:) delegate method is called).

## See Also

### Related Documentation

@MainActor func deauthorize(_ inSender: Any!) -> Bool

Sets the authorization state to unauthorized and locks the lock icon in the view.

