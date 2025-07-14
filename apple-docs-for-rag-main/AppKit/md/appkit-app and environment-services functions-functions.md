

- AppKit
- App and Environment
-  Services Functions 

API Collection

# Services Functions

Configure the contents of your app’s Services menu.

## Topics

### Registering Services

func NSRegisterServicesProvider(Any?, NSServiceProviderName)

Registers a service provider.

func NSUnregisterServicesProvider(NSServiceProviderName)

Unregisters a service provider.

func NSUpdateDynamicServices()

Causes the services information for the system to be updated.

typealias NSServiceProviderName

### Performing Services

func NSPerformService(String, NSPasteboard?) -> Bool

Programmatically invokes a Services menu service.

## See Also

### App Services

class NSSharingService

An object that facilitates the sharing of content with social media services, or with apps like Mail or Safari.

class NSSharingServicePicker

A list of sharing services that the user can choose from.

protocol NSPreviewRepresentableActivityItem

An interface you adopt in custom objects that you want to share using the macOS share sheet.

class NSSharingServicePickerToolbarItem

A toolbar item that displays the macOS share sheet.

protocol NSServicesMenuRequestor

A set of methods that support interaction with items users can share through a sharing service.

protocol NSCloudSharingServiceDelegate

A set of methods for responding to the life cycle events of the cloud-sharing service.

