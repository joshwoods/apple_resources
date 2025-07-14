

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  complete(authorizationResult:) 

Instance Method

# complete(authorizationResult:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
func complete(authorizationResult: ASAuthorizationProviderExtensionAuthorizationResult)
```

## See Also

### Completing a Request

func complete()

Indicates the requested authorization completed with no output.

func complete(httpAuthorizationHeaders: [String : String])

Indicates the requested authorization succeeded with tokens in the HTTP headers.

func complete(httpResponse: HTTPURLResponse, httpBody: Data?)

Indicates the requested authorization succeeded with an HTTP response.

func complete(error: any Error)

Indicates the requested authorization failed.

