

- Shared With You Core
- SWCollaborationMetadata
-  collaborationIdentifier 

Instance Property

# collaborationIdentifier

A globally unique identifier that the app hosting the collaboration provides.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var collaborationIdentifier: SWCollaborationIdentifier { get }
```

## Discussion

This identifier is unique across platforms and sharing sessions.

## See Also

### Accessing metadata attributes

var defaultShareOptions: SWCollaborationShareOptions?

The collaboration options that the content supports.

var initiatorHandle: String?

The handle of the person who initiates the collaboration.

var initiatorNameComponents: PersonNameComponents?

The name of the person who initiates the collaboration.

var localIdentifier: SWLocalCollaborationIdentifier

A locally unique identifier for the item the metadata represents.

var title: String?

The title of the content.

var userSelectedShareOptions: SWCollaborationShareOptions?

The selected collaboration options from the person who sends the invitation.

