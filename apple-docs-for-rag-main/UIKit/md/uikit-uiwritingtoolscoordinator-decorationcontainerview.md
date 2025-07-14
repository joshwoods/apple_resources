

- UIKit
- UIWritingToolsCoordinator
-  decorationContainerView 

Instance Property

# decorationContainerView

The view that Writing Tools uses to display background decorations such as proofreading marks.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
weak var decorationContainerView: UIView? { get set }
```

## Discussion

Writing Tools uses the view in this property to host proofreading marks and other visual elements that show any suggested changes. Set this property to a subview situated visibly below the text in your custom text view. It’s also satisfactory to place this view visually in front of the text. Make sure the size of the view is big enough to cover all of the affected text. If you don’t assign a value to this property, the coordinator uses the object in its view property to host any visual elements.

If you display your view’s text using multiple text containers, implement the writingToolsCoordinator(_:requestsSingleContainerSubrangesOf:in:completion:) and writingToolsCoordinator(_:requestsDecorationContainerViewFor:in:completion:) methods to provide separate decoration views for each container.

## See Also

### Getting the host views for effects

var effectContainerView: UIView?

The view that Writing Tools uses to display visual effects during the text-rewriting process.

