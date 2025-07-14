

- Authentication Services
- ASAccountAuthenticationModificationControllerPresentationContextProviding
-  presentationAnchor(for:) 

Instance Method

# presentationAnchor(for:)

Returns the most appropriate window for presenting the authentication modification interface.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
func presentationAnchor(for controller: ASAccountAuthenticationModificationController) -> ASPresentationAnchor
```

**Required**

## Parameters 

`controller`  

The controller that performs the account authentication modification request.

## Return Value

A window to present the authentication modification interface.

