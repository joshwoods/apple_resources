

- Shared With You Core
- SWCollaborationMetadata
-  userSelectedShareOptions 

Instance Property

# userSelectedShareOptions

The selected collaboration options from the person who sends the invitation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
@NSCopying
var userSelectedShareOptions: SWCollaborationShareOptions? { get set }
```

## Mentioned in 

Adding custom collaboration to your app

## See Also

### Accessing metadata attributes

var collaborationIdentifier: SWCollaborationIdentifier

A globally unique identifier that the app hosting the collaboration provides.

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

