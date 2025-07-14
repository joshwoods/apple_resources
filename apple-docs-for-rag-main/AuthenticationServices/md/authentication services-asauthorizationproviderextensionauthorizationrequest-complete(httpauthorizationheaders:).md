

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  complete(httpAuthorizationHeaders:) 

Instance Method

# complete(httpAuthorizationHeaders:)

Indicates the requested authorization succeeded with tokens in the HTTP headers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
func complete(httpAuthorizationHeaders: [String : String])
```

## Parameters 

`httpAuthorizationHeaders`  

The collection of tokens from the header.

## See Also

### Completing a Request

func complete(authorizationResult: ASAuthorizationProviderExtensionAuthorizationResult)

func complete()

Indicates the requested authorization completed with no output.

func complete(httpResponse: HTTPURLResponse, httpBody: Data?)

Indicates the requested authorization succeeded with an HTTP response.

func complete(error: any Error)

Indicates the requested authorization failed.

