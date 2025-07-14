

- AVFoundation
- AVPlayerItemLegibleOutput
-  textStylingResolution 

Instance Property

# textStylingResolution

A string identifier indicating the degree of text styling to be applied to attributed strings vended by the object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var textStylingResolution: AVPlayerItemLegibleOutput.TextStylingResolution { get set }
```

## Discussion

Valid values are described in `Text Style Settings`. An exception (invalidArgumentException) is raised if this property is set to any other value.

The default value is default, which indicates that attributed strings vended by the receiver includes the same level of styling information that would be used if the text was rendered by an instance of AVPlayerLayer.

Note

This is an advanced feature and you should rarely need to change it from the default value.

## See Also

### Configuring Text Styling

struct TextStylingResolution

A text styling resolution.

