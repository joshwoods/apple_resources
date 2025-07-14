

- CarPlay
- CPActionSheetTemplate
-  init(title:message:actions:) 

Initializer

# init(title:message:actions:)

Creates an action sheet template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    title: String?,
    message: String?,
    actions: [CPAlertAction]
)
```

## Parameters 

`title`  

The title of the action sheet.

`message`  

A descriptive message providing details about the reason for displaying the action sheet.

`actions`  

A list of actions available on the action sheet. The array must contain at least one action.

## Return Value

A newly initialized action sheet template.

