

- Device Management
-  AppManagedInstallBehavior_LicenseObject 

Object

# AppManagedInstallBehavior_LicenseObject

A dictionary that specifies the type of license the app uses.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
object AppManagedInstallBehavior_LicenseObject
```

## Properties

`Assignment`

`string`

Possible Values: `Device, User`

`VPPType`

`string`

The type of VPP license that the app uses for installation through the App Store, which is one of the following values:

Device  
The app has a VPP device license.

User  
The app has a VPP user license.

This key needs to be present to install an app through the App Store.

Possible Values: `Device, User`

