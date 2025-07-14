

- Shared With You Core
- SWCollaborationMetadata
-  initiatorNameComponents 

Instance Property

# initiatorNameComponents

The name of the person who initiates the collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var initiatorNameComponents: PersonNameComponents? { get set }
```

## Discussion

The app that initiates a collaboration sets the `initiatorNameComponents` to allow the user to confirm the components before the system begins the collaboration. The value of the components will not be transmitted to recipients, and is `nil` before the system initiates a collaboration.

## See Also

### Accessing metadata attributes

var collaborationIdentifier: SWCollaborationIdentifier

A globally unique identifier that the app hosting the collaboration provides.

var defaultShareOptions: SWCollaborationShareOptions?

The collaboration options that the content supports.

var initiatorHandle: String?

The handle of the person who initiates the collaboration.

var localIdentifier: SWLocalCollaborationIdentifier

A locally unique identifier for the item the metadata represents.

var title: String?

The title of the content.

var userSelectedShareOptions: SWCollaborationShareOptions?

The selected collaboration options from the person who sends the invitation.

