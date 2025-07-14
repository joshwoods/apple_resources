

- UIKit
- UITextViewDelegate
-  textView(\_:textItemMenuWillDisplayFor:animator:) 

Instance Method

# textView(\_:textItemMenuWillDisplayFor:animator:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    textItemMenuWillDisplayFor textItem: UITextItem,
    animator: any UIContextMenuInteractionAnimating
)
```

## See Also

### Interacting with text data

func textView(UITextView, menuConfigurationFor: UITextItem, defaultMenu: UIMenu) -> UITextItem.MenuConfiguration?

func textView(UITextView, primaryActionFor: UITextItem, defaultAction: UIAction) -> UIAction?

func textView(UITextView, textItemMenuWillEndFor: UITextItem, animator: any UIContextMenuInteractionAnimating)

