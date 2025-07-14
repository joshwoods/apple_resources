

- Create ML
- MLSoundClassifier
- MLSoundClassifier.DataSource
-  labeledSounds() 

Instance Method

# labeledSounds()

Generates a dictionary of the data source’s labeled audio files.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+visionOS 1.0+

``` source
func labeledSounds() throws -> [String : [URL]]
```

## Return Value

A dictionary of labeled audio files. Each dictionary key is a label string and its value is an array of audio-file URLs.

