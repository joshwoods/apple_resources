

- Device Management
- AutonomousSingleAppMode
-  AutonomousSingleAppMode.AllowedApplicationsItem 

Device Management Profile

# AutonomousSingleAppMode.AllowedApplicationsItem

A dictionary that specifies an app that can be granted access to the Accessibilty APIs.

macOS 10.13.4+Device Assignment ServicesVPP License Management

``` source
object AutonomousSingleAppMode.AllowedApplicationsItem
```

## Properties

`BundleIdentifier`

`string`

 (Required) 

The unique bundle identifier.

`TeamIdentifier`

`string`

 (Required) 

The developer’s team identifier that the system used when it signed the app.

## Discussion

Important

If two dictionaries contain the same `BundleIdentifier` value but a different `TeamIdentifier` value, an error occurs and the system doesn’t install the profile.

