

- Device Management
- AppLock
-  AppLock.App 

Device Management Profile

# AppLock.App

The only app available for use on the iOS device.

iOS 6.0+iPadOS 6.0+tvOS 10.2+Device Assignment ServicesVPP License Management

``` source
object AppLock.App
```

## Properties

`Identifier`

`string`

 (Required) 

The app’s bundle identifier.

`Options`

AppLock.App.Options

A dictionary of options that the user can’t change.

`UserEnabledOptions`

AppLock.App.UserEnabledOptions

A dictionary of user-editable options.

## Topics

### Profiles

object AppLock.App.Options

The dictionary of options to set for the app.

object AppLock.App.UserEnabledOptions

The dictionary of user-editable options to set for the app.

