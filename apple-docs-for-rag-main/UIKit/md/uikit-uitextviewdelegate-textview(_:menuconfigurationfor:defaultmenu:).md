

- UIKit
- UITextViewDelegate
-  textView(\_:menuConfigurationFor:defaultMenu:) 

Instance Method

# textView(\_:menuConfigurationFor:defaultMenu:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
optional func textView(
    _ textView: UITextView,
    menuConfigurationFor textItem: UITextItem,
    defaultMenu: UIMenu
) -> UITextItem.MenuConfiguration?
```

## See Also

### Interacting with text data

func textView(UITextView, primaryActionFor: UITextItem, defaultAction: UIAction) -> UIAction?

func textView(UITextView, textItemMenuWillDisplayFor: UITextItem, animator: any UIContextMenuInteractionAnimating)

func textView(UITextView, textItemMenuWillEndFor: UITextItem, animator: any UIContextMenuInteractionAnimating)

