

- AVFAudio
-  AVAudioNodeTapBlock 

Type Alias

# AVAudioNodeTapBlock

The block that receives copies of the output of an audio node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVAudioNodeTapBlock = (AVAudioPCMBuffer, AVAudioTime) -> Void
```

## Parameters 

`buffer`  

A buffer of audio the system captures from the output of an audio node`.`

`when`  

The time the system captures the buffer.

## Discussion

Important

The framework may invoke this callback on a thread other than the main thread.

## See Also

### Installing and Removing an Audio Tap

func installTap(onBus: AVAudioNodeBus, bufferSize: AVAudioFrameCount, format: AVAudioFormat?, block: AVAudioNodeTapBlock)

Installs an audio tap on a bus you specify to record, monitor, and observe the output of the node.

func removeTap(onBus: AVAudioNodeBus)

Removes an audio tap on a bus you specify.

