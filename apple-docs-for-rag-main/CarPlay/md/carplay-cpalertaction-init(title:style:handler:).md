

- CarPlay
- CPAlertAction
-  init(title:style:handler:) 

Initializer

# init(title:style:handler:)

Creates an alert action with a title, style, and action handler.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    title: String,
    style: CPAlertAction.Style,
    handler: @escaping CPAlertActionHandler
)
```

## Parameters 

`title`  

The title displayed on the action button.

`style`  

The display style for the action button.

`handler`  

The block invoked after the user taps the action button.

## Return Value

A newly initialized alert action.

