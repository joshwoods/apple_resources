

- TV Services
- TVTopShelfCarouselItem
-  mediaOptions 

Instance Property

# mediaOptions

Information about the media format and presentation options.

tvOS 13.0+

``` source
var mediaOptions: TVTopShelfCarouselItem.MediaOptions { get set }
```

## Discussion

Specify all of the options that apply to the underlying content. The system adds standard icons for the options you support. For example, if you specify the videoResolution4K option, the system adds an icon to the detail view indicating that playback in 4K resolution is possible.

## See Also

### Adding Media Badges

struct MediaOptions

Constants indicating the item’s audio and video capabilities.

