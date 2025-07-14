

- Shared With You Core
- SWCollaborationCoordinator
-  actionHandler 

Instance Property

# actionHandler

The collaboration action handler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
weak var actionHandler: (any SWCollaborationActionHandler)? { get set }
```

## Discussion

Register the delegate soon after launch and handle actions immediately to avoid timeouts.

## See Also

### Accessing coordinator attributes

class var shared: SWCollaborationCoordinator

The shared collaboration coordinator.

