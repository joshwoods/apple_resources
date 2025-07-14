

- AVFAudio
- AVAudioUnitComponentManager
-  components(passingTest:) 

Instance Method

# components(passingTest:)

Gets an array of audio components that pass the block method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func components(passingTest testHandler: @escaping (AVAudioUnitComponent, UnsafeMutablePointer) -> Bool) -> [AVAudioUnitComponent]
```

## Parameters 

`testHandler`  

The block to apply to the audio unit components.

The block takes two parameters.

comp  
A block to test.

stop  
A reference to a Boolean value. To stop further processing of the search, the block sets the value to true. The stop argument is an out-only argument. Only set this Boolean to true within the block.

The block returns a Boolean value that indicates whether `comp` passes the test. Returning true stops further processing of the audio components.

## Return Value

An array of audio components that pass the test.

## Discussion

For each audio component the manager finds, the system calls the block method. If the block returns true, the method adds `AVAudioComponent` instance to the array.

## See Also

### Getting matching audio components

func components(matching: AudioComponentDescription) -> [AVAudioUnitComponent]

Gets an array of audio component objects that match the description.

func components(matching: NSPredicate) -> [AVAudioUnitComponent]

Gets an array of audio component objects that match the search predicate.

