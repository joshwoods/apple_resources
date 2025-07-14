

- Device Management
- Notifications
-  Notifications.NotificationSettingsItem 

Device Management Profile

# Notifications.NotificationSettingsItem

The notification settings dictionary.

iOS 9.3+iPadOS 9.3+macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object Notifications.NotificationSettingsItem
```

## Properties

`AlertType`

`integer`

The type of alert for notifications for this app:

- `0`: None

- `1`: Temporary Banner

- `2`: Persistent Banner

Available in iOS 9.3 and later and macOS 10.15 and later.

Default: `1`

Possible Values: `0, 1, 2`

`BadgesEnabled`

`boolean`

If `true`, enables badges for this app.

Available in iOS 9.3 and later and macOS 10.15 and later.

Default: `true`

`BundleIdentifier`

`string`

 (Required) 

The bundle identifier of the app to which to apply these notification settings.

Available in iOS 9.3 and later and macOS 10.15 and later.

`CriticalAlertEnabled`

`boolean`

If `true`, enables critical alerts that can ignore Do Not Disturb and ringer settings for this app.

Available in iOS 12 and later and macOS 10.15 and later.

Default: `false`

`GroupingType`

`integer`

The type of grouping for notifications for this app:

- `0`: Automatic: Group notifications into app-specified groups.

- `1`: By app: Group notifications into one group.

- `2`: Off: Don’t group notifications.

Available in iOS 12 and later.

Default: `0`

Possible Values: `0, 1, 2`

`NotificationsEnabled`

`boolean`

If `true`, enables notifications for this app.

Available in iOS 9.3 and later and macOS 10.15 and later.

Default: `true`

`PreviewType`

`integer`

The type previews for notifications. This key overrides the value at Settings\>Notifications\>Show Previews.

- `0` - Always: Previews will be shown when the device is locked and unlocked

- `1` - When Unlocked: Previews will only be shown when the device is unlocked

- `2` - Never: Previews will never be shown

Available in iOS 14 and later.

Possible Values: `0, 1, 2`

`ShowInCarPlay`

`boolean`

If `true`, enables notifications in CarPlay for this app.

Available in iOS 12 and later.

Default: `true`

`ShowInLockScreen`

`boolean`

If `true`, enables notifications on the lock screen for this app.

Available in iOS 9.3 and later and macOS 10.15 and later.

Default: `true`

`ShowInNotificationCenter`

`boolean`

If `true`, enables notifications in the notification center for this app.

Available in iOS 9.3 and later and macOS 10.15 and later.

Default: `true`

`SoundsEnabled`

`boolean`

If `true`, enables sounds for this app.

Default: `true`

