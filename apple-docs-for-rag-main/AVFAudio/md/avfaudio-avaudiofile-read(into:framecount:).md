

- AVFAudio
- AVAudioFile
-  read(into:frameCount:) 

Instance Method

# read(into:frameCount:)

Reads a portion of an audio buffer using the number of frames you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func read(
    into buffer: AVAudioPCMBuffer,
    frameCount frames: AVAudioFrameCount
) throws
```

## Parameters 

`buffer`  

The buffer from which to read the file. Its format must match the file’s processing format.

`frames`  

The number of frames to read.

## Discussion

You use this method to read fewer frames than the buffer’s `frameCapacity`.

## See Also

### Reading and Writing the Audio Buffer

func read(into: AVAudioPCMBuffer) throws

Reads an entire audio buffer.

func write(from: AVAudioPCMBuffer) throws

Writes an audio buffer sequentially.

func close()

Closes the audio file.

