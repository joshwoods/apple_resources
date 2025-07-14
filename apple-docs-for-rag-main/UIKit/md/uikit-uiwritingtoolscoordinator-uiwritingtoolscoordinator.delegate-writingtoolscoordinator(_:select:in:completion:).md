

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.Delegate
-  writingToolsCoordinator(\_:select:in:completion:) 

Instance Method

# writingToolsCoordinator(\_:select:in:completion:)

Asks the delegate to update your view’s current text selection.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    select ranges: [NSValue],
    in context: UIWritingToolsCoordinator.Context,
    completion: @escaping () -> Void
)
```

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    select ranges: [NSValue],
    in context: UIWritingToolsCoordinator.Context
) async
```

**Required**

## Parameters 

`writingToolsCoordinator`  

The coordinator object making the change to your view.

`ranges`  

One or more ranges of text to select. Each range is relative to the text in your context object, and it’s your responsibility to match each location to the correct location in your text storage. If you initialized the context object with the entire contents of your view’s text storage, you can use the ranges as-is to access that text storage. However, if you initialized the context object with only a portion of your view’s text, add the starting location of your context object’s text to each value to get the correct range for that text storage.

`context`  

The context object you use to identify the associated text storage.

`completion`  

The completion handler to execute when your delegate finishes updating the selection. The handler has no parameters or return value. You must call this handler at some point during the implementation of your method.

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

As Writing Tools suggests changes to your view’s text, it calls this method to update the text selection accordingly. Use this method to update the current selection in your view’s text storage. When you finish making the changes, call the provided completion block to let Writing Tools know you’re finished.

## See Also

### Incorporating Writing Tools suggestions

func writingToolsCoordinator(UIWritingToolsCoordinator, replace: NSRange, in: UIWritingToolsCoordinator.Context, proposedText: NSAttributedString, reason: UIWritingToolsCoordinator.TextReplacementReason, animationParameters: UIWritingToolsCoordinator.AnimationParameters?, completion: (NSAttributedString?) -> Void)

Tells the delegate that there are text changes to incorporate into the view.

**Required**

