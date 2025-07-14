

- AVFoundation
- AVPlayerItem
-  outputs 

Instance Property

# outputs

An array of outputs associated with the player item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
@MainActor
var outputs: [AVPlayerItemOutput] { get }
```

## Discussion

This property contains the collection of AVPlayerItemOutput objects used to transfer media data to the player object.

## See Also

### Managing Player Item Outputs

func add(AVPlayerItemOutput)

Adds the specified player item output object to the receiver.

func remove(AVPlayerItemOutput)

Removes the specified player item output object from the receiver.

