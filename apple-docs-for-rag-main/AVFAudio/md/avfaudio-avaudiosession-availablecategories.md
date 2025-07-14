

- AVFAudio
- AVAudioSession
-  availableCategories 

Instance Property

# availableCategories

The audio session categories available on the current device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var availableCategories: [AVAudioSession.Category] { get }
```

## Discussion

Not every device supports every audio session category. For instance, the record category isn’t available on a device that doesn’t support audio input.

Query this property to determine if the category you’d like to use is available on the current device.

## See Also

### Inspecting the category configuration

var category: AVAudioSession.Category

The current audio session category.

struct Category

Audio session category identifiers.

var categoryOptions: AVAudioSession.CategoryOptions

The set of options associated with the current audio session category.

struct CategoryOptions

Constants that specify optional audio behaviors.

