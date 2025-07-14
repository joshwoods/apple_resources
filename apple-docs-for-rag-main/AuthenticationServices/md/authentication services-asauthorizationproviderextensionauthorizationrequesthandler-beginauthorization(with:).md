

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequestHandler
-  beginAuthorization(with:) 

Instance Method

# beginAuthorization(with:)

Tells your request handler to authorize the given request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
func beginAuthorization(with request: ASAuthorizationProviderExtensionAuthorizationRequest)
```

**Required**

## Parameters 

`request`  

The request to be authorized.

## Discussion

The system calls this method on the main thread.

## See Also

### Starting or Canceling a Request

func cancelAuthorization(with: ASAuthorizationProviderExtensionAuthorizationRequest)

Tells your request handler to cancel the authorization of the given request.

class ASAuthorizationProviderExtensionAuthorizationRequest

An authorization request that your provider extension handles.

