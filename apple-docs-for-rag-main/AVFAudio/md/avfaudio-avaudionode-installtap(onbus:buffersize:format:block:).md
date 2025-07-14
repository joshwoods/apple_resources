

- AVFAudio
- AVAudioNode
-  installTap(onBus:bufferSize:format:block:) 

Instance Method

# installTap(onBus:bufferSize:format:block:)

Installs an audio tap on a bus you specify to record, monitor, and observe the output of the node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func installTap(
    onBus bus: AVAudioNodeBus,
    bufferSize: AVAudioFrameCount,
    format: AVAudioFormat?,
    block tapBlock: @escaping AVAudioNodeTapBlock
)
```

## Parameters 

`bus`  

The output bus to attach the tap to.

`bufferSize`  

The size of the incoming buffers. The implementation may choose another size.

`format`  

If non-`nil`, the framework applies this format to the output bus you specify. An error occurs when attaching to an output bus that’s already in a connected state. The tap and connection formats (if non-`nil`) on the bus need to be identical. Otherwise, the latter operation overrides the previous format.

For `AVAudioOutputNode`, you must specify the tap format as `nil`.

`tapBlock`  

A block the framework calls with audio buffers.

## Discussion

You can install and remove taps while the engine is in a running state. You can install only one tap on any bus.

```
```

Important

The framework may invoke the `tapBlock` on a thread other than the main thread.

## See Also

### Installing and Removing an Audio Tap

func removeTap(onBus: AVAudioNodeBus)

Removes an audio tap on a bus you specify.

typealias AVAudioNodeTapBlock

The block that receives copies of the output of an audio node.

