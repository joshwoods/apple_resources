

- UIKit
- UIWritingToolsCoordinator
- UIWritingToolsCoordinator.Delegate
-  writingToolsCoordinator(\_:replace:in:proposedText:reason:animationParameters:completion:) 

Instance Method

# writingToolsCoordinator(\_:replace:in:proposedText:reason:animationParameters:completion:)

Tells the delegate that there are text changes to incorporate into the view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    replace range: NSRange,
    in context: UIWritingToolsCoordinator.Context,
    proposedText replacementText: NSAttributedString,
    reason: UIWritingToolsCoordinator.TextReplacementReason,
    animationParameters: UIWritingToolsCoordinator.AnimationParameters?,
    completion: @escaping (NSAttributedString?) -> Void
)
```

``` source
func writingToolsCoordinator(
    _ writingToolsCoordinator: UIWritingToolsCoordinator,
    replace range: NSRange,
    in context: UIWritingToolsCoordinator.Context,
    proposedText replacementText: NSAttributedString,
    reason: UIWritingToolsCoordinator.TextReplacementReason,
    animationParameters: UIWritingToolsCoordinator.AnimationParameters?
) async -> NSAttributedString?
```

**Required**

## Parameters 

`writingToolsCoordinator`  

The coordinator object providing the changes to your custom view.

`range`  

A range of text to update. This range is relative to the text in your context object, and it’s your responsibility to match that location to the correct location in your text storage. If you initialized the context object with the entire contents of your view’s text storage, you can use `range` as-is to access that text storage. However, if you initialized the context object with only a portion of your view’s text, add the starting location of your context object’s text to this value to get the correct range for that text storage.

`context`  

The context object that contains the original text to modify. Use this object to locate the correct text storage object for your view.

`replacementText`  

The text to insert in place of the current text at `range`. You can insert this text as-is, insert a modified version of this string, or reject the replacement text altogether.

`reason`  

The type of replacement Writing Tools performs. This parameter indicates whether Writing Tools is replacing the text with or without animations.

`animationParameters`  

The animation parameters for any interactive changes, or `nil` if the changes aren’t interactive. Use this object to create any additional animations for the system to run alongside the changes Writing Tools makes. For example, use it to update other views that contain related information.

`completion`  

A completion handler to execute with the results of the operation. The handler has no return value and takes an optional attributed string as a parameter. If you incorporate the replacement text, either as-is or with modifications, pass the actual string you incorporated to the completion block. If you reject the suggested change and leave the original text unchanged, specify `nil` for this parameter.

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

Use this method to update your view’s text storage with the proposed changes. Writing Tools can call this method multiple times during the course of a session to notify you of changes to different ranges of text. Incorporate the changes into your view’s text storage and notify your layout manager so it can refresh the view.

Important

When integrating changes, remember to update `range.location` as needed to get the correct location in your view’s text storage.

Remove the text in the appropriate range of your text storage, and replace it with the contents of `replacementText`. When you finish, call the completion handler and pass in the replacement text you inserted. If you change the string in `replacementText` before incorporating it into your text storage, return your modified string instead. Returning the string lets Writing Tools track any alterations you made to it. You can also pass `nil` to the completion handler if you don’t incorporate the replacement text.

For interactive changes, Writing Tools works with your delegate to animate the removal of the old text and the insertion of any replacement text. If you need to modify other parts of your interface to reflect the changes, use the provided UIWritingToolsCoordinator.AnimationParameters object to create additional animations to run at the same time as the system-provided animations.

## See Also

### Incorporating Writing Tools suggestions

func writingToolsCoordinator(UIWritingToolsCoordinator, select: [NSValue], in: UIWritingToolsCoordinator.Context, completion: () -> Void)

Asks the delegate to update your view’s current text selection.

**Required**

