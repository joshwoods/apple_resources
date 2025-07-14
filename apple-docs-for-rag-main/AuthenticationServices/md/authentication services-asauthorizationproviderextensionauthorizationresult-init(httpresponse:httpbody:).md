

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationResult
-  init(httpResponse:httpBody:) 

Initializer

# init(httpResponse:httpBody:)

Initializes an authorization with a HTTP response and body.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    httpResponse: HTTPURLResponse,
    httpBody: Data?
)
```

## Parameters 

`httpResponse`  

The HTTP response.

`httpBody`  

The HTTP body.

## See Also

### Initializers

init(httpAuthorizationHeaders: [String : String])

Initializes an authorization with tokens stored in HTTP headers.

