

- ARKit
- ARSession
-  update(with:) 

Instance Method

# update(with:)

Updates your session with information about the physical environment that is collected by another user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func update(with collaborationData: ARSession.CollaborationData)
```

## Discussion

Call this function to update a session when the app receives collaboration data from other users that are participating in a multiuser AR experience. Your app receives this data when multiple users scan different parts of an environment and share that information with your app over the network. For more information, see isCollaborationEnabled.

Collaboration is supported for world tracking configurations only.

## See Also

### Managing collaboration

class CollaborationData

An object that holds information that a user has collected about the physical environment.

