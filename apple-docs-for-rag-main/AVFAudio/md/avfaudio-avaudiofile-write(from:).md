

- AVFAudio
- AVAudioFile
-  write(from:) 

Instance Method

# write(from:)

Writes an audio buffer sequentially.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(from buffer: AVAudioPCMBuffer) throws
```

## Parameters 

`buffer`  

The buffer from which to write to the file. Its format must match the file’s processing format.

## Discussion

The buffer’s frameLength signifies how much of the buffer the method writes.

## See Also

### Reading and Writing the Audio Buffer

func read(into: AVAudioPCMBuffer) throws

Reads an entire audio buffer.

func read(into: AVAudioPCMBuffer, frameCount: AVAudioFrameCount) throws

Reads a portion of an audio buffer using the number of frames you specify.

func close()

Closes the audio file.

