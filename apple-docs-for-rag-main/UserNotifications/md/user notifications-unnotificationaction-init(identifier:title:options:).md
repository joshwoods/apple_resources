

- User Notifications
- UNNotificationAction
-  init(identifier:title:options:) 

Initializer

# init(identifier:title:options:)

Creates an action object by using the specified title and options.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    identifier: String,
    title: String,
    options: UNNotificationActionOptions = []
)
```

## Parameters 

`identifier`  

The string that you use internally to identify the action. This string must be unique among your app’s supported actions. When the user selects the action, the system passes this string to your app and asks the user to perform the related task. This parameter must not be `nil` or an empty string.

`title`  

The localized string the system displays to the user. The system displays this string as the title of a button, which the system adds to the notification interface. This parameter must not be `nil`.

`options`  

Additional options that describe how the action behaves. Include options when you need the related behavior. For a list of possible values, see UNNotificationActionOptions.

## Return Value

An action object that the system initializes.

## See Also

### Essentials

convenience init(identifier: String, title: String, options: UNNotificationActionOptions, icon: UNNotificationActionIcon?)

Creates an action object by using the specified title, options, and icon.

