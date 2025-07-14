

- WatchKit
- WKAlertAction
-  init(title:style:handler:) 

Initializer

# init(title:style:handler:)

Creates and returns an action object with the specified button information.

watchOS 2.0+

``` source
convenience init(
    title: String,
    style: WKAlertActionStyle,
    handler: @escaping WKAlertActionHandler
)
```

## Parameters 

`title`  

The localized string to use as the button title for the action.

`style`  

The style to apply to the action button. For a list of possible styles and their meanings, see WKAlertActionStyle.

`handler`  

A block containing the code to execute when the user taps the action button. Use this block to perform whatever action is required to perform the associated task. For information about the format of this block, see WKAlertActionHandler.

## Return Value

An initialized action object that you can display in an alert.

## Discussion

Use this method to create a button to display in an action sheet. In an action sheet, specifying an action with the WKAlertActionStyle.cancel style replaces the standard Cancel button provided by the system.

