

- Shared With You
- SWHighlightCenter
-  isSystemCollaborationSupportAvailable 

Type Property

# isSystemCollaborationSupportAvailable

A Boolean value that represents full support for Messages collaboration features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class var isSystemCollaborationSupportAvailable: Bool { get }
```

## See Also

### Retrieving collaboration highlights

func collaborationHighlight(forIdentifier: SWCollaborationIdentifier) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified collaboration identifier.

func collaborationHighlight(forIdentifier: String) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified identifier string.

func getCollaborationHighlight(for: URL, completionHandler: (SWCollaborationHighlight?, (any Error)?) -> Void)

Returns a collaboration highlight for a specified URL.

func getHighlightFor(URL, completionHandler: (SWHighlight?, (any Error)?) -> Void)

Returns a highlight for a specified URL.

func getSignedIdentityProof(for: SWCollaborationHighlight, using: Data, completionHandler: (SWPerson.SignedIdentityProof?, (any Error)?) -> Void)

Signs passed-in data with the local device’s private key.

