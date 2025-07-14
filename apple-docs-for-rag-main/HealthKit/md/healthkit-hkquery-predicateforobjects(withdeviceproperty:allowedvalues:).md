

- HealthKit
- HKQuery
-  predicateForObjects(withDeviceProperty:allowedValues:) 

Type Method

# predicateForObjects(withDeviceProperty:allowedValues:)

Returns a predicate that matches all objects created by devices with the specified properties.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func predicateForObjects(
    withDeviceProperty key: String,
    allowedValues: Set
) -> NSPredicate
```

## Parameters 

`key`  

A string specifying the device’s property. For a list of valid keys, see Valid Device Property Keys.

`allowedValues`  

A set of strings. These strings represent the target property values.

## Return Value

A predicate that matches all objects created by a device whose specified property matches one of the allowed values.

## Discussion

Use this convenience method to create a predicate that finds all the objects saved by matching devices. These predicates let you match multiple values for a single property. For example, you can create a single predicate that matches a number of different `manufacturer` values.

The following sample shows how to create a predicate that matches a list of device model names.

- Swift
- Objective-C

```
let fromDevices = HKQuery.predicateForObjectsWithDeviceProperty(HKDevicePropertyKeyModel, allowedValues:modelNames)
```

```
NSPredicate *fromDevices = [HKQuery predicateForObjectsWithDeviceProperty:HKDevicePropertyKeyModel allowedValues:modelNames];
```

## Topics

### Valid Device Property Keys

Use these keys to create predicates that match the specified device property.

let HKDevicePropertyKeyName: String

The device’s name.

let HKDevicePropertyKeyManufacturer: String

The device’s manufacturer.

let HKDevicePropertyKeyModel: String

The device’s model.

let HKDevicePropertyKeyHardwareVersion: String

The device’s hardware version.

let HKDevicePropertyKeyFirmwareVersion: String

The device’s firmware version.

let HKDevicePropertyKeySoftwareVersion: String

The device’s software version.

let HKDevicePropertyKeyLocalIdentifier: String

A unique identifier for the device on the hardware running the app. For more information, see localIdentifier.

let HKDevicePropertyKeyUDIDeviceIdentifier: String

The device’s UDI Device Identifier.

## See Also

### Creating object predicates

class func predicateForObject(with: UUID) -> NSPredicate

Returns a predicate that matches an object with the specified universally unique identifier (UUID).

class func predicateForObjects(with: Set&lt;UUID>) -> NSPredicate

Returns a predicate that matches the objects with the specified universally unique identifiers (UUIDs).

class func predicateForObjects(from: HKSource) -> NSPredicate

Returns a predicate that matches all the objects that were created by the provided source.

class func predicateForObjects(from: Set&lt;HKSource>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided sources.

class func predicateForObjects(from: Set&lt;HKDevice>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided devices.

class func predicateForObjects(from: Set&lt;HKSourceRevision>) -> NSPredicate

Returns a predicate that matches all the objects that were created by any of the provided source revisions.

class func predicateForObjects(withMetadataKey: String) -> NSPredicate

Returns a predicate that matches any object whose metadata contains the provided key.

class func predicateForObjects(withMetadataKey: String, allowedValues: [Any]) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key and an array of target values.

class func predicateForObjects(withMetadataKey: String, operatorType: NSComparisonPredicate.Operator, value: Any) -> NSPredicate

Returns a predicate that matches objects based on the provided metadata key, value, and operator.

class func predicateForObjectsWithNoCorrelation() -> NSPredicate

Returns a predicate that matches all objects that are not associated with a HealthKit correlation.

