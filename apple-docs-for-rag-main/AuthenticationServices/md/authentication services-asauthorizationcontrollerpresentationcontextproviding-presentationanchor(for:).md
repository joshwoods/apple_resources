

- Authentication Services
- ASAuthorizationControllerPresentationContextProviding
-  presentationAnchor(for:) 

Instance Method

# presentationAnchor(for:)

Tells the delegate from which window it should present content to the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func presentationAnchor(for controller: ASAuthorizationController) -> ASPresentationAnchor
```

**Required**

## Parameters 

`controller`  

The controller asking for the presentation anchor.

## Return Value

A user interface element that can act as the anchor for the authorization presentation.

## See Also

### Specifying the Anchor

typealias ASPresentationAnchor

A platform-specific type that indicates the kind of user interface element to use as a presentation anchor.

