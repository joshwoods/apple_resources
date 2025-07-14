

- AVFAudio
- AVAudioUnitComponentManager
-  components(matching:) 

Instance Method

# components(matching:)

Gets an array of audio component objects that match the description.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func components(matching desc: AudioComponentDescription) -> [AVAudioUnitComponent]
```

## Return Value

An array of `AVAudioComponent` objects that match the `description`.

## Discussion

- desc: The AudioComponentDescription structure to match. The method uses the `type`, `subtype` and `manufacturer` fields to search for matching audio units. A value of `0` for any of these fields is a wildcard and returns the first match the method finds.

## See Also

### Getting matching audio components

func components(matching: NSPredicate) -> [AVAudioUnitComponent]

Gets an array of audio component objects that match the search predicate.

func components(passingTest: (AVAudioUnitComponent, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> [AVAudioUnitComponent]

Gets an array of audio components that pass the block method.

