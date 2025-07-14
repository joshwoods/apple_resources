

- AVFAudio
- AVAudioSession
-  supportsMultichannelContent 

Instance Property

# supportsMultichannelContent

A Boolean value that indicates whether your app supplies multichannel audio content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var supportsMultichannelContent: Bool { get }
```

## Discussion

The default value is `false`.

## See Also

### Configuring multichannel support

func setSupportsMultichannelContent(Bool) throws

Sets whether your app supplies multichannel audio content.

