

- Shared With You Core
- SWCollaborationMetadata
-  defaultShareOptions 

Instance Property

# defaultShareOptions

The collaboration options that the content supports.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@NSCopying
var defaultShareOptions: SWCollaborationShareOptions? { get set }
```

## Mentioned in 

Adding custom collaboration to your app

## See Also

### Accessing metadata attributes

var collaborationIdentifier: SWCollaborationIdentifier

A globally unique identifier that the app hosting the collaboration provides.

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

