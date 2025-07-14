

- SecureElementCredential
- CredentialSession
-  invalidate() 

Instance Method

# invalidate()

Inmediately invalidates a session.

iOS 18.1+iPadOS 18.1+

``` source
func invalidate() async throws
```

## Discussion

Call this method when your app no longer needs a credential session. The system automatically invalidates a session when it deallocates, or when it encounters underlying errors.

When a session invalidates, its event stream also invalidates and deallocates.

You can invalidate a session while in any session state.

## See Also

### Managing the credential session life cycle

static func startSession() async throws -> CredentialSession

Requests a session to view, manage, or use credentials in the Secure Element.

