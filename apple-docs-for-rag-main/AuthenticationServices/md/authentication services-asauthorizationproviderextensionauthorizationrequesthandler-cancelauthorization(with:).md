

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequestHandler
-  cancelAuthorization(with:) 

Instance Method

# cancelAuthorization(with:)

Tells your request handler to cancel the authorization of the given request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
@MainActor
optional func cancelAuthorization(with request: ASAuthorizationProviderExtensionAuthorizationRequest)
```

## Parameters 

`request`  

The request to cancel.

## Discussion

The system calls this method on the main thread.

## See Also

### Starting or Canceling a Request

func beginAuthorization(with: ASAuthorizationProviderExtensionAuthorizationRequest)

Tells your request handler to authorize the given request.

**Required**

class ASAuthorizationProviderExtensionAuthorizationRequest

An authorization request that your provider extension handles.

