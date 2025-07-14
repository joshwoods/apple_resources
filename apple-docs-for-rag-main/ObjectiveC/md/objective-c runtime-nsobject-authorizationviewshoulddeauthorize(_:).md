

- Objective-C Runtime
- NSObject
-  authorizationViewShouldDeauthorize(\_:) 

Instance Method

# authorizationViewShouldDeauthorize(\_:)

Sent to the delegate when a user clicks the open lock icon.

macOS 10.3+

``` source
func authorizationViewShouldDeauthorize(_ view: SFAuthorizationView!) -> Bool
```

## Discussion

The delegate can react to this before deauthorization happens and avoid it by returning NO. This delegate method is not called when you call the deauthorize(_:) method.

## See Also

### Related Documentation

@MainActor func deauthorize(_ inSender: Any!) -> Bool

Sets the authorization state to unauthorized and locks the lock icon in the view.

