

- AVFoundation
- AVPlayerItem
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified player item output object from the receiver.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
@MainActor
func remove(_ output: AVPlayerItemOutput)
```

## Parameters 

`output`  

The player item output object to remove.

## See Also

### Managing Player Item Outputs

var outputs: [AVPlayerItemOutput]

An array of outputs associated with the player item.

func add(AVPlayerItemOutput)

Adds the specified player item output object to the receiver.

