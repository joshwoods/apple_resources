

- Shared With You Core
- SWStartCollaborationAction
-  fulfill(using:collaborationIdentifier:) 

Instance Method

# fulfill(using:collaborationIdentifier:)

Informs an app to set up the universal link and device independent identifier to provide to the system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func fulfill(
    using url: URL,
    collaborationIdentifier: SWCollaborationIdentifier
)
```

## Parameters 

`url`  

The universal link to give to the system.

`collaborationIdentifier`  

The SWCollaborationIdentifier to give to the system.

