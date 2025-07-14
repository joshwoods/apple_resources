

- TV Services
-  TVTopShelfCarouselItem 

Class

# TVTopShelfCarouselItem

An item containing images, video, and other information that you want to display using a carousel-based interface.

tvOS 13.0+

``` source
class TVTopShelfCarouselItem
```

## Overview

A TVTopShelfCarouselItem object offers a more dynamic way to present your content than section-based items. When a carousel item first appears, it displays either a static image or a short looping video as its background. When the navigation focus stops on the item, the system plays the video in the item’s previewVideoURL property.

Create one or more TVTopShelfCarouselItem objects and fill them with information about your content. The system determines which properties of the object to display based on the content style. For the TVTopShelfCarouselContent.Style.details style, the system displays all of the information in your carousel item. For the TVTopShelfCarouselContent.Style.actions style, the system focuses on the actions associated with your item. To specify the actions for both styles, use the inherited playAction and displayAction properties of the object.

## Topics

### Specifying the Item Details

var contextTitle: String?

A localized string describing why the item is shown in the top shelf.

var summary: String?

A descriptive summary of a movie or show.

var genre: String?

The genre assigned to the movie or show.

var duration: TimeInterval

The length of the movie or show, in seconds.

var creationDate: Date?

The original release date of the content.

### Specifying the Content Previews

var cinemagraphURL: URL?

The URL of a looping video to play, without sound, while the preview loads.

var previewVideoURL: URL?

The URL for the content’s trailer or preview.

### Adding Media Badges

var mediaOptions: TVTopShelfCarouselItem.MediaOptions

Information about the media format and presentation options.

struct MediaOptions

Constants indicating the item’s audio and video capabilities.

### Adding Custom Attributes

var namedAttributes: [TVTopShelfNamedAttribute]

Additional information to display for your content, such as a list of leading actors.

class TVTopShelfNamedAttribute

An object you use to display additional information.

## Relationships

### Inherits From

- TVTopShelfItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Carousel content

class TVTopShelfCarouselContent

A set of items you present using a carousel-style interface in the top shelf.

