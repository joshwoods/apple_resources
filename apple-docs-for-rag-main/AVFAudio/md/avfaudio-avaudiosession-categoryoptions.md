

- AVFAudio
- AVAudioSession
-  categoryOptions 

Instance Property

# categoryOptions

The set of options associated with the current audio session category.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var categoryOptions: AVAudioSession.CategoryOptions { get }
```

## Discussion

You use category options to tailor the behavior of the active audio session category. See AVAudioSession.CategoryOptions for the supported values.

## See Also

### Inspecting the category configuration

var category: AVAudioSession.Category

The current audio session category.

var availableCategories: [AVAudioSession.Category]

The audio session categories available on the current device.

struct Category

Audio session category identifiers.

struct CategoryOptions

Constants that specify optional audio behaviors.

