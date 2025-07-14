

- AVKit
- AVMultiviewManager
-  contentSelectionViewController 

Instance Property

# contentSelectionViewController

A view controller that presents a user interface to select additional video content to display.

visionOS 2.0+

``` source
@MainActor
final var contentSelectionViewController: AVContentSelectionViewController? { get set }
```

## Discussion

Implement this property to add custom user interface elements. The primary role of this interface is to provide a way for users to add additional videos.

## See Also

### Providing additional UI

class AVContentSelectionViewController

A view controller for providing additional UI to the multiview experience.

