

- AVFAudio
- AVAudioUnitComponentManager
-  components(matching:) 

Instance Method

# components(matching:)

Gets an array of audio component objects that match the search predicate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func components(matching predicate: NSPredicate) -> [AVAudioUnitComponent]
```

## Parameters 

`predicate`  

The search predicate.

## Return Value

An array of `AVAudioComponent` objects that match the predicate.

## Discussion

You use the audio component’s information or tags to build search criteria, such as `“typeName CONTAINS 'Effect'"` or `“tags IN {'Sampler', 'MIDI'}"`.

## See Also

### Getting matching audio components

func components(matching: AudioComponentDescription) -> [AVAudioUnitComponent]

Gets an array of audio component objects that match the description.

func components(passingTest: (AVAudioUnitComponent, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [AVAudioUnitComponent]

Gets an array of audio components that pass the block method.

