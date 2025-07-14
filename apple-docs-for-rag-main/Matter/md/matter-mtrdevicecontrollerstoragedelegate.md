

- Matter
-  MTRDeviceControllerStorageDelegate 

Protocol

# MTRDeviceControllerStorageDelegate

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
protocol MTRDeviceControllerStorageDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func controller(MTRDeviceController, removeValueForKey: String, securityLevel: MTRStorageSecurityLevel, sharingType: MTRStorageSharingType) -> Bool

**Required**

func controller(MTRDeviceController, storeValue: any NSSecureCoding, forKey: String, securityLevel: MTRStorageSecurityLevel, sharingType: MTRStorageSharingType) -> Bool

**Required**

func controller(MTRDeviceController, storeValues: [String : any NSSecureCoding], securityLevel: MTRStorageSecurityLevel, sharingType: MTRStorageSharingType) -> Bool

func controller(MTRDeviceController, valueForKey: String, securityLevel: MTRStorageSecurityLevel, sharingType: MTRStorageSharingType) -> (any NSSecureCoding)?

**Required**

func values(for: MTRDeviceController, securityLevel: MTRStorageSecurityLevel, sharingType: MTRStorageSharingType) -> [String : any NSSecureCoding]?

## Relationships

### Inherits From

- NSObjectProtocol

