

- Media Player
- MPRemoteCommandHandlerStatus
-  MPRemoteCommandHandlerStatus.deviceNotFound 

Case

# MPRemoteCommandHandlerStatus.deviceNotFound

The requested command couldn’t execute because a required device isn’t available.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
case deviceNotFound
```

## Discussion

Commands that require a device to perform their action should return this status when the device is unavailable. For example, you’d return this status if your command requires headphones, but none are available.

## See Also

### Constants

case success

The requested command executed successfully.

case noSuchContent

The requested command couldn’t execute because its required content isn’t available.

case noActionableNowPlayingItem

The requested command couldn’t execute because no Now Playing item is available.

case commandFailed

The requested command failed to execute.

