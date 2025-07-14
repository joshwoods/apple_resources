

- Shared With You Core
- SWCollaborationActionHandler
-  collaborationCoordinator(\_:handle:) 

Instance Method

# collaborationCoordinator(\_:handle:)

Notifies the delegate when the system updates the participants in a collaboration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func collaborationCoordinator(
    _ coordinator: SWCollaborationCoordinator,
    handle action: SWUpdateCollaborationParticipantsAction
)
```

**Required**

## Parameters 

`coordinator`  

The SWCollaborationCoordinator for this action.

`action`  

The SWStartCollaborationAction for this collaboration.

## See Also

### Handling collaboration actions

func collaborationCoordinator(SWCollaborationCoordinator, handle: SWStartCollaborationAction)

Notifies the delegate when the system starts a collaboration.

**Required**

