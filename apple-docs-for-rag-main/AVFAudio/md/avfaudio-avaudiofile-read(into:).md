

- AVFAudio
- AVAudioFile
-  read(into:) 

Instance Method

# read(into:)

Reads an entire audio buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func read(into buffer: AVAudioPCMBuffer) throws
```

## Parameters 

`buffer`  

The buffer from which to read the file. Its format must match the file’s processing format.

## Discussion

When reading sequentially from the framePosition property, the method attempts to fill the buffer to its capacity. On return, the buffer’s length property indicates the number of sample frames it successfully reads.

## See Also

### Related Documentation

var framePosition: AVAudioFramePosition

The position in the file where the next read or write operation occurs.

var length: AVAudioFramePosition

The number of sample frames in the file.

### Reading and Writing the Audio Buffer

func read(into: AVAudioPCMBuffer, frameCount: AVAudioFrameCount) throws

Reads a portion of an audio buffer using the number of frames you specify.

func write(from: AVAudioPCMBuffer) throws

Writes an audio buffer sequentially.

func close()

Closes the audio file.

