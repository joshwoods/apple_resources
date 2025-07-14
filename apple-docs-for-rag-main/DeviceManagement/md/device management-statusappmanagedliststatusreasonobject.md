

- Device Management
-  StatusAppManagedListStatusReasonObject 

Object

# StatusAppManagedListStatusReasonObject

A dictionary that contains details about a declarative managed app’s state.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object StatusAppManagedListStatusReasonObject
```

## Properties

`code`

`string`

 (Required) 

A code for the state.

`description`

`string`

A description of the state.

`details`

StatusAppManagedListStatusReason_DetailsObject

A dictionary that contains additional details about the state.

## Discussion

A `StatusAppManagedListStatusReasonObject` has the following possible values:

`Error.AppStoreDisabled`  
The system disabled the App Store.

`Error.DuplicateConfiguredApp`  
The system is already managing the app.

`Error.DownloadFailed`  
The app download failed. The `details` dictionary contains a `Timestamp` key with the RFC 3339 timestamp of the last download failure.

`Error.InstallFailed`  
The app install failed. The `details` dictionary contains a `Timestamp` key with the RFC 3339 timestamp of the last install failure.

`Error.InvalidAppID`  
The system couldn’t find the app ID.

`Error.LicenseNotFound`  
A license for the app isn’t available.

`Error.NotAnApp`  
The downloaded data isn’t a valid app.

`Error.NotSupported`  
The app isn’t supported on the device.

`Error.UnmanagedAppAlreadyInstalled`  
An unmanaged version of the app that the system can’t manage is already installed.

`Error.UpdateFailed`  
The app update failed. The `details` dictionary contains a `Timestamp` key with the RFC 3339 timestamp of the last update failure.

`Error.UserRejected`  
The user rejected management of the app.

`Info.UpdateAvailable`  
An update is available for the app.

## Topics

### Objects

object StatusAppManagedListStatusReason_DetailsObject

A dictionary that contains additional details about a declarative managed app’s error state.

object StatusAppManagedListManagedConfigurationObject

A dictionary that contains details about a declarative managed app’s managed configuration.

## See Also

### Objects

object StatusAppManagedListManagedConfigurationObject

A dictionary that contains details about a declarative managed app’s managed configuration.

