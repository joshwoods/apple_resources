

- UIKit
- UITextDraggable
-  textDragInteraction 

Instance Property

# textDragInteraction

The drag interaction object added by UIKit to the text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var textDragInteraction: UIDragInteraction? { get }
```

**Required**

## Discussion

You can set the text drag interaction’s isEnabled property to false if you need to explicitly turn off drag interactions for a UIKit-provided text view.

