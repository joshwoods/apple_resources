

- UIKit
- UIAlertController
-  init(title:message:preferredStyle:) 

Initializer

# init(title:message:preferredStyle:)

Creates and returns a view controller for displaying an alert.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    title: String?,
    message: String?,
    preferredStyle: UIAlertController.Style
)
```

## Parameters 

`title`  

The title of the alert. Use this string to get people’s attention and communicate the reason for the alert.

`message`  

Descriptive text that provides additional details about the reason for the alert.

`preferredStyle`  

The style to use when presenting the alert controller. Use this parameter to configure the alert controller as an action sheet or as a modal alert.

## Return Value

An initialized alert controller object.

## Discussion

After creating the alert controller, configure any actions that you want people to be able to perform by calling the addAction(_:) method one or more times. When specifying a preferred style of UIAlertController.Style.alert, you may also configure one or more text fields to display in addition to the actions.

