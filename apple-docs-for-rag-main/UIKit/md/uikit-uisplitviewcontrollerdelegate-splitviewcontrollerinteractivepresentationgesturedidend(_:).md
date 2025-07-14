

- UIKit
- UISplitViewControllerDelegate
-  splitViewControllerInteractivePresentationGestureDidEnd(\_:) 

Instance Method

# splitViewControllerInteractivePresentationGestureDidEnd(\_:)

Tells the delegate when the interactive presentation gesture ends.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
optional func splitViewControllerInteractivePresentationGestureDidEnd(_ svc: UISplitViewController)
```

## Parameters 

`svc`  

The split view controller responding to the interactive presentation gesture.

## Discussion

This delegate method only applies to column-style split view interfaces. For more information, see Split view styles.

The split view controller calls this method when the interactive presentation gesture ends. Use this method for performance optimizations related to drawing the column content or other work related to handling the interactive gesture.

## See Also

### Handling the presentation gesture

func splitViewControllerInteractivePresentationGestureWillBegin(UISplitViewController)

Tells the delegate that the interactive presentation gesture is about to begin.

