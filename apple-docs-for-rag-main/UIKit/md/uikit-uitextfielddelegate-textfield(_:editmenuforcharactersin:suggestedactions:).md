

- UIKit
- UITextFieldDelegate
-  textField(\_:editMenuForCharactersIn:suggestedActions:) 

Instance Method

# textField(\_:editMenuForCharactersIn:suggestedActions:)

Asks the delegate for the menu to display in the text field, based on the text range and actions the system provides.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
optional func textField(
    _ textField: UITextField,
    editMenuForCharactersIn range: NSRange,
    suggestedActions: [UIMenuElement]
) -> UIMenu?
```

## Parameters 

`textField`  

The text field requesting the menu.

`range`  

The character range the menu is presenting for.

`suggestedActions`  

The actions and commands the system suggests.

## Return Value

Returns a menu describing the desired menu hierarchy. Return `nil` to present the default system menu.

## Discussion

The following example returns a menu that includes a “Show in Large Type” action.

```
func textField(_ textField: UITextField, editMenuForCharactersIn range: NSRange, suggestedActions: [UIMenuElement]) -> UIMenu? {
    let showLargeAction = UIAction(title: "Show in Large Type", image: UIImage(systemName: "a.magnify")) { action in
            // Include "Show in Large Type" action.
    }

    var actions = suggestedActions
    actions.append(showLargeAction)
    return UIMenu(children: actions)
}
```

