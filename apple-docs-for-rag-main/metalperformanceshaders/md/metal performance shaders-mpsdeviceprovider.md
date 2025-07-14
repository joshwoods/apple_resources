

- Metal Performance Shaders
-  MPSDeviceProvider 

Protocol

# MPSDeviceProvider

An interface that enables the setting of a Metal device for unarchived objects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol MPSDeviceProvider
```

## Topics

### Instance Methods

func mpsMTLDevice() -> (any MTLDevice)!

**Required**

## Relationships

### Conforming Types

- MPSKeyedUnarchiver

## See Also

### Keyed Archivers

class NSKeyedArchiver

An encoder that stores an object’s data to an archive referenced by keys.

class MPSKeyedUnarchiver

A keyed archiver that supports Metal Performance Shaders kernel decoding.

