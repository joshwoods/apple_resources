

- Core Media I/O
-  CMIOExtensionProviderProperties 

Class

# CMIOExtensionProviderProperties

An object that manages the properties of an extension provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionProviderProperties
```

## Overview

Create an instance of this object to manage the provider’s property state.

## Topics

### Creating Provider Properties

init(dictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Creates a provider properties object with the specified properties.

### Managing Properties

var name: String?

The provider name.

var manufacturer: String?

The provider manufacturer.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets a state value for the specified property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a provider.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Providers

Creating a camera extension with Core Media I/O

Build high-performance camera drivers that are secure and simple to deploy.

Overriding the default USB video class extension

Create a simple DriverKit extension to override the default driver-matching behavior for USB devices.

class CMIOExtensionProvider

An object that manages device connections for a provider.

protocol CMIOExtensionProviderSource

A protocol for objects that act as provider sources.

