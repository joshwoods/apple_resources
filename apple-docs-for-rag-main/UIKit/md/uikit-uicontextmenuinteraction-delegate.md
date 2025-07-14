

- UIKit
- UIContextMenuInteraction
-  delegate 

Instance Property

# delegate

The object that provides the preview and contextual menu for your content and responds to interaction-related events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIContextMenuInteractionDelegate)? { get }
```

## See Also

### Previewing and managing the content

protocol UIContextMenuInteractionDelegate

The methods for providing the set of actions to perform on your content, and for customizing the preview of that content.

