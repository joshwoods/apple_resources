

- TV Services
- TVTopShelfCarouselItem
-  previewVideoURL 

Instance Property

# previewVideoURL

The URL for the content’s trailer or preview.

tvOS 13.0+

``` source
var previewVideoURL: URL? { get set }
```

## Discussion

When the navigation focus stops on the item, the system removes the item’s static image or cinemagraph video and plays the video at the specified URL.

## See Also

### Specifying the Content Previews

var cinemagraphURL: URL?

The URL of a looping video to play, without sound, while the preview loads.

