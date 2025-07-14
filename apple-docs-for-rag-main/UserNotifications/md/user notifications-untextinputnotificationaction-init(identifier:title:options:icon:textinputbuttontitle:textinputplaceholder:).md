

- User Notifications
- UNTextInputNotificationAction
-  init(identifier:title:options:icon:textInputButtonTitle:textInputPlaceholder:) 

Initializer

# init(identifier:title:options:icon:textInputButtonTitle:textInputPlaceholder:)

Creates an action object with an icon that accepts text input from the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(
    identifier: String,
    title: String,
    options: UNNotificationActionOptions = [],
    icon: UNNotificationActionIcon?,
    textInputButtonTitle: String,
    textInputPlaceholder: String
)
```

## Parameters 

`identifier`  

The string that you use internally to identify the action. This string must be unique among all of your app’s supported actions. When the user selects the action, the system passes this string to your app and asks you to perform the related task. This parameter must not be `nil` or an empty string.

`title`  

The localized string the system displays to the user. The system displays this string as the title of a button, which the system adds to the notification interface. This parameter must not be `nil`.

`options`  

Additional options describing how the action behaves. Include options when you need the related behavior. For a list of possible values, see UNNotificationActionOptions.

`icon`  

The icon to display to the user.

`textInputButtonTitle`  

The localized title of the text input button that’s displayed to the user.

`textInputPlaceholder`  

The localized placeholder text to display in the text input field.

## Return Value

A new text input action object.

## See Also

### Essentials

convenience init(identifier: String, title: String, options: UNNotificationActionOptions, textInputButtonTitle: String, textInputPlaceholder: String)

Creates an action object that accepts text input from the user.

