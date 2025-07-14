

- Metal Performance Shaders
-  MPSKeyedUnarchiver 

Class

# MPSKeyedUnarchiver

A keyed archiver that supports Metal Performance Shaders kernel decoding.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSKeyedUnarchiver : NSKeyedUnarchiver
```

## Topics

### Initializers

init?(device: any MTLDevice)Deprecated

init(forReadingFrom: Data, device: any MTLDevice, error: NSErrorPointer)

init(forReadingWith: Data, device: any MTLDevice)Deprecated

### Instance Methods

func mpsMTLDevice() -> any MTLDevice

### Type Methods

class func unarchiveObject(with: Data, device: any MTLDevice) -> Any?Deprecated

class func unarchiveObject(withFile: String, device: any MTLDevice) -> Any?Deprecated

class func unarchiveTopLevelObject(with: Data, device: any MTLDevice) -> AnyDeprecated

class func unarchivedObject(of: AnyClass, from: Data, device: any MTLDevice) -> Any

class func unarchivedObject(ofClasses: Set&lt;AnyHashable>, from: Data, device: any MTLDevice) -> Any

## Relationships

### Inherits From

- NSKeyedUnarchiver

### Conforms To

- MPSDeviceProvider

## See Also

### Keyed Archivers

class NSKeyedArchiver

An encoder that stores an object’s data to an archive referenced by keys.

protocol MPSDeviceProvider

An interface that enables the setting of a Metal device for unarchived objects.

