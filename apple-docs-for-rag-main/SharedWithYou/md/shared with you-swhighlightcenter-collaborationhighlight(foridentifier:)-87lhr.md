

- Shared With You
- SWHighlightCenter
-  collaborationHighlight(forIdentifier:) 

Instance Method

# collaborationHighlight(forIdentifier:)

Returns a collaboration highlight for a specified identifier string.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS

``` source
func collaborationHighlight(forIdentifier: String) throws -> SWCollaborationHighlight
```

## Parameters 

`forIdentifier`  

The unique identifier that the system uses to find the SWCollaborationHighlight.

## Return Value

The `SWCollaborationHighlight` associated with the `identifier`.

## See Also

### Retrieving collaboration highlights

class var isSystemCollaborationSupportAvailable: Bool

A Boolean value that represents full support for Messages collaboration features.

func collaborationHighlight(forIdentifier: SWCollaborationIdentifier) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified collaboration identifier.

func getCollaborationHighlight(for: URL, completionHandler: (SWCollaborationHighlight?, (any Error)?) -> Void)

Returns a collaboration highlight for a specified URL.

func getHighlightFor(URL, completionHandler: (SWHighlight?, (any Error)?) -> Void)

Returns a highlight for a specified URL.

func getSignedIdentityProof(for: SWCollaborationHighlight, using: Data, completionHandler: (SWPerson.SignedIdentityProof?, (any Error)?) -> Void)

Signs passed-in data with the local device’s private key.

