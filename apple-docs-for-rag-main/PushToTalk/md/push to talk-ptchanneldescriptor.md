

- Push to Talk
-  PTChannelDescriptor 

Class

# PTChannelDescriptor

An object that describes a channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
class PTChannelDescriptor
```

## Mentioned in 

Creating a Push to Talk app

## Topics

### Creating a channel descriptor

init(name: String, image: UIImage?)

Creates a channel descriptor with the name and image you specify.

### Inspecting a channel descriptor

var name: String

The channel name that the system presents in the system user interface.

var image: UIImage?

The channel photo that the system presents in the user interface to represent the channel.

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
- Sendable

## See Also

### Channel restoration

protocol PTChannelRestorationDelegate

A type that represents the channel restoration behavior.

