

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationResult
-  init(httpAuthorizationHeaders:) 

Initializer

# init(httpAuthorizationHeaders:)

Initializes an authorization with tokens stored in HTTP headers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(httpAuthorizationHeaders: [String : String])
```

## Parameters 

`httpAuthorizationHeaders`  

The HTTP authorization headers.

## See Also

### Initializers

init(httpResponse: HTTPURLResponse, httpBody: Data?)

Initializes an authorization with a HTTP response and body.

