

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  complete(httpResponse:httpBody:) 

Instance Method

# complete(httpResponse:httpBody:)

Indicates the requested authorization succeeded with an HTTP response.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
func complete(
    httpResponse: HTTPURLResponse,
    httpBody: Data?
)
```

## Parameters 

`httpResponse`  

The metadata associated with the HTTP response.

`httpBody`  

The body of the HTTP response.

## See Also

### Completing a Request

func complete(authorizationResult: ASAuthorizationProviderExtensionAuthorizationResult)

func complete()

Indicates the requested authorization completed with no output.

func complete(httpAuthorizationHeaders: [String : String])

Indicates the requested authorization succeeded with tokens in the HTTP headers.

func complete(error: any Error)

Indicates the requested authorization failed.

