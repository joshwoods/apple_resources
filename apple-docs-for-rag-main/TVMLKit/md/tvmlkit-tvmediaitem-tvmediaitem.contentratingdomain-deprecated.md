

- TVMLKit
- TVMediaItem
-  TVMediaItem.ContentRatingDomain Deprecated

Structure

# TVMediaItem.ContentRatingDomain

A value identifying the media’s content rating domain.

tvOS 12.0–18.0Deprecated

``` source
struct ContentRatingDomain
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Rating Domains

static let movie: TVMediaItem.ContentRatingDomain

The media item’s rating uses the movie domain.

static let music: TVMediaItem.ContentRatingDomain

The media item’s rating uses the music domain.

static let tvShow: TVMediaItem.ContentRatingDomain

The media item’s rating uses the TV show domain.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Rating Media Content

var containsExplicitContent: Bool

A Boolean value indicating whether the item contains adult-oriented content.

Deprecated

var contentRatingDomain: TVMediaItem.ContentRatingDomain?

The media domain that the rating applies to.

Deprecated

var contentRatingRanking: NSNumber?

The rating for a video item.

Deprecated

