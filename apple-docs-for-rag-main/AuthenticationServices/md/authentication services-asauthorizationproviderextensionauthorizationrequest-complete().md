

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  complete() 

Instance Method

# complete()

Indicates the requested authorization completed with no output.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
func complete()
```

## See Also

### Completing a Request

func complete(authorizationResult: ASAuthorizationProviderExtensionAuthorizationResult)

func complete(httpAuthorizationHeaders: [String : String])

Indicates the requested authorization succeeded with tokens in the HTTP headers.

func complete(httpResponse: HTTPURLResponse, httpBody: Data?)

Indicates the requested authorization succeeded with an HTTP response.

func complete(error: any Error)

Indicates the requested authorization failed.

