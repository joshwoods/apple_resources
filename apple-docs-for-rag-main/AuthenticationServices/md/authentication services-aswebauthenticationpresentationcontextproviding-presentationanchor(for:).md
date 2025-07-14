

- Authentication Services
- ASWebAuthenticationPresentationContextProviding
-  presentationAnchor(for:) 

Instance Method

# presentationAnchor(for:)

Tells the delegate from which window it should present content to the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
@MainActor
func presentationAnchor(for session: ASWebAuthenticationSession) -> ASPresentationAnchor
```

**Required**

## Parameters 

`session`  

The session asking for the presentation anchor.

## Return Value

A user interface element that can act as the anchor for the authentication presentation.

## Mentioned in 

Authenticating a User Through a Web Service

## See Also

### Specifying the Anchor

typealias ASPresentationAnchor

A platform-specific type that indicates the kind of user interface element to use as a presentation anchor.

