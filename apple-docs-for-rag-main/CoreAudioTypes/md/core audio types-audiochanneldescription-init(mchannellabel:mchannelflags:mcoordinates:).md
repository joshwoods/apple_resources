

- Core Audio Types
- AudioChannelDescription
-  init(mChannelLabel:mChannelFlags:mCoordinates:) 

Initializer

# init(mChannelLabel:mChannelFlags:mCoordinates:)

Creates a channel description with a label, flags, and coordinates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mChannelLabel: AudioChannelLabel,
    mChannelFlags: AudioChannelFlags,
    mCoordinates: (Float32, Float32, Float32)
)
```

## Parameters 

`mChannelLabel`  

A label for the chanel.

`mChannelFlags`  

The flags to set for a channel.

`mCoordinates`  

The coordinates.

## See Also

### Creating a Channel Description

init()

Creates an empty channel description.

