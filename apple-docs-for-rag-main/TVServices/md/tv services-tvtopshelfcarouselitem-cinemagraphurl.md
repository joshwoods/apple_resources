

- TV Services
- TVTopShelfCarouselItem
-  cinemagraphURL 

Instance Property

# cinemagraphURL

The URL of a looping video to play, without sound, while the preview loads.

tvOS 13.0+

``` source
var cinemagraphURL: URL? { get set }
```

## Discussion

If you specify a value for this property, the system initially displays the corresponding video instead of a static image. The video plays in a loop until the preview video loads and is ready to play. If you do not specify a value for this property, the system displays the image you set using the setImageURL(_:for:) method.

The system does not play any sound content present in the video, so there is no need to include it when creating your assets.

## See Also

### Specifying the Content Previews

var previewVideoURL: URL?

The URL for the content’s trailer or preview.

