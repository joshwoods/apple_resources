

- Objective-C Runtime
- NSObject
-  authorizationViewCreatedAuthorization(\_:) 

Instance Method

# authorizationViewCreatedAuthorization(\_:)

Sent to the delegate to indicate the authorization object has been created or changed.

macOS 10.3+

``` source
func authorizationViewCreatedAuthorization(_ view: SFAuthorizationView!)
```

## Discussion

If you have saved a copy of the authorization object for your own purposes, you should discard it and call authorization() for a new authorization object.

