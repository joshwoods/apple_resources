

- Shared With You Core
- SWCollaborationMetadata
-  localIdentifier 

Instance Property

# localIdentifier

A locally unique identifier for the item the metadata represents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var localIdentifier: SWLocalCollaborationIdentifier { get }
```

## Mentioned in 

Adding custom collaboration to your app

## Discussion

Use this identifier to uniquely identify this metadata before the system creates a collaborationIdentifier.

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

var title: String?

The title of the content.

var userSelectedShareOptions: SWCollaborationShareOptions?

The selected collaboration options from the person who sends the invitation.

