

- Shared With You
- SWHighlightCenter
-  getCollaborationHighlight(for:completionHandler:) 

Instance Method

# getCollaborationHighlight(for:completionHandler:)

Returns a collaboration highlight for a specified URL.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func getCollaborationHighlight(
    for URL: URL,
    completionHandler: @escaping (SWCollaborationHighlight?, (any Error)?) -> Void
)
```

``` source
func collaborationHighlight(for URL: URL) async throws -> SWCollaborationHighlight
```

## Parameters 

`URL`  

The URL that the system uses to find the SWCollaborationHighlight.

`completionHandler`  

Returns the SWCollaborationHighlight. The system invokes the completion handler on the main thread.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func collaborationHighlight(for URL: URL) async throws -> SWCollaborationHighlight
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Retrieving collaboration highlights

class var isSystemCollaborationSupportAvailable: Bool

A Boolean value that represents full support for Messages collaboration features.

func collaborationHighlight(forIdentifier: SWCollaborationIdentifier) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified collaboration identifier.

func collaborationHighlight(forIdentifier: String) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified identifier string.

func getHighlightFor(URL, completionHandler: (SWHighlight?, (any Error)?) -> Void)

Returns a highlight for a specified URL.

func getSignedIdentityProof(for: SWCollaborationHighlight, using: Data, completionHandler: (SWPerson.SignedIdentityProof?, (any Error)?) -> Void)

Signs passed-in data with the local device’s private key.

