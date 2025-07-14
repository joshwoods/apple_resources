

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.Delegate
-  writingToolsCoordinator(\_:requestsPreviewFor:of:in:completion:) 

Instance Method

# writingToolsCoordinator(\_:requestsPreviewFor:of:in:completion:)

Asks the delegate for a preview image and layout information for the specified text.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    requestsPreviewFor textAnimation: UIWritingToolsCoordinator.TextAnimation,
    of range: NSRange,
    in context: UIWritingToolsCoordinator.Context,
    completion: @escaping (UITargetedPreview?) -> Void
)
```

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    previewFor textAnimation: UIWritingToolsCoordinator.TextAnimation,
    range: NSRange,
    context: UIWritingToolsCoordinator.Context
) async -> UITargetedPreview?
```

**Required**

## Parameters 

`writingToolsCoordinator`  

The coordinator object notifying you that animations are about to begin.

`textAnimation`  

The type of animation Writing Tools is preparing.

`range`  

The range of text that requires a preview image. This range is relative to the text in your context object, and it’s your responsibility to match that location to the correct location in your text storage. If you initialized the context object with the entire contents of your view’s text storage, you can use `range` as-is to access that text storage. However, if you initialized the context object with only a portion of your view’s text, add the starting location of your context object’s text to this value to get the correct range for that text storage.

`context`  

The context object that contains the original text. Use this object to fetch the current text, and to match that text to your underlying text storage.

`completion`  

A completion handler to execute when you are done. The handler has no return value and takes a UITargetedPreview object as a parameter. You must call this handler at some point during your implementation.

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

During an interactive evaluation of your view’s text, Writing Tools creates different animations to provide feedback on what’s happening. As part of the preparation for those animations, Writing Tools asks you to provide a preview of the affected content in your view. Writing Tools uses this preview to build and execute the animations in the view stored in the effectContainerView property of the coordinator object.

To build a preview of your content in iOS, render the specified range of text into an image with a transparent background. Install the image in a UIImageView and use that to build your preview object. Set the frame rectangle of your image view to the rectangle in your view’s coordinate space that contains the text you captured. When creating the UITargetedPreview object, include both a UIPreviewParameters and a UIPreviewTarget object. Create the UIPreviewTarget object with your text view as the container, and set the center point to the center of your text view. Create the UIPreviewParameters object using the selection rectangles for the text, which you get from your view’s layout manager. Writing Tools uses this information to place your image directly above the text in your view.

For a single animation type, the system calls this method, followed sequentially by the `writingToolsCoordinator(_:prepareFor:range:context:completion:)` and writingToolsCoordinator(_:finish:for:in:completion:) methods. Each method executes asynchronously, but the system calls the next method in the sequence only after you call the completion handler of the previous method. However, multiple animations can run simultaneously, so check the `textAnimation` parameter to differentiate sequences.

## See Also

### Animating inline text changes

func writingToolsCoordinator(UIWritingToolsCoordinator, prepareFor: UIWritingToolsCoordinator.TextAnimation, for: NSRange, in: UIWritingToolsCoordinator.Context, completion: () -> Void)

Prepare for animations for the content that Writing Tools is evaluating.

**Required**

func writingToolsCoordinator(UIWritingToolsCoordinator, finish: UIWritingToolsCoordinator.TextAnimation, for: NSRange, in: UIWritingToolsCoordinator.Context, completion: () -> Void)

Asks the delegate to clean up any state related to the specified Writing Tools animation.

**Required**

