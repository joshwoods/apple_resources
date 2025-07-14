

- Push to Talk
-  PTChannelRestorationDelegate 

Protocol

# PTChannelRestorationDelegate

A type that represents the channel restoration behavior.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
protocol PTChannelRestorationDelegate : NSObjectProtocol
```

## Mentioned in 

Creating a Push to Talk app

## Topics

### Getting the channel descriptor

func channelDescriptor(restoredChannelUUID: UUID) -> PTChannelDescriptor

Tells your observer the system restored the channel.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Channel restoration

class PTChannelDescriptor

An object that describes a channel.

