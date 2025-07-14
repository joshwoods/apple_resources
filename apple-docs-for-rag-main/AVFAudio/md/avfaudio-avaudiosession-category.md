

- AVFAudio
- AVAudioSession
-  category 

Instance Property

# category

The current audio session category.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var category: AVAudioSession.Category { get }
```

## Discussion

An audio session category defines a set of audio behaviors for your app. The default category assigned to an audio session is soloAmbient.

## See Also

### Inspecting the category configuration

var availableCategories: [AVAudioSession.Category]

The audio session categories available on the current device.

struct Category

Audio session category identifiers.

var categoryOptions: AVAudioSession.CategoryOptions

The set of options associated with the current audio session category.

struct CategoryOptions

Constants that specify optional audio behaviors.

