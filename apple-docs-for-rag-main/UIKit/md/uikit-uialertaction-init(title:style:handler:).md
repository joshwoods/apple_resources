

- UIKit
- UIAlertAction
-  init(title:style:handler:) 

Initializer

# init(title:style:handler:)

Create and return an action with the specified title and behavior.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    title: String?,
    style: UIAlertAction.Style,
    handler: ((UIAlertAction) -> Void)? = nil
)
```

## Parameters 

`title`  

The text to use for the button title. The value you specify should be localized for the user’s current language. This parameter must not be `nil`, except in a tvOS app where a `nil` title may be used with UIAlertAction.Style.cancel.

`style`  

Additional styling information to apply to the button. Use the style information to convey the type of action that is performed by the button. For a list of possible values, see the constants in UIAlertAction.Style.

`handler`  

A block to execute when the user selects the action. This block has no return value and takes the selected action object as its only parameter.

## Return Value

A new alert action object.

## Discussion

Actions are enabled by default when you create them.

