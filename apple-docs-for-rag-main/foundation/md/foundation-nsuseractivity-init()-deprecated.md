

- Foundation
- NSUserActivity
-  init() Deprecated

Initializer

# init()

Creates a user activity object using the first activity type declared in the app’s information property list file.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
convenience init()
```

Deprecated

Use initWithActivityType: with a specific activity type string

## Return Value

An NSUserActivity object.

## Discussion

This method retrieves the first string of the NSUserActivityTypes key declared in the app’s `Info.plist` file.

## See Also

### Creating a user activity object

Creating a user activity object

Identify key user interactions and include the information to restore them later.

init(activityType: String)

Creates a user activity object with the specified type.

