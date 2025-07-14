

- TVMLKit
- TVMediaItem
-  contentRatingRanking Deprecated

Instance Property

# contentRatingRanking

The rating for a video item.

tvOS 12.0–18.0Deprecated

``` source
var contentRatingRanking: NSNumber? { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

The rating is a value from `0-1000`. This value corresponds to a specific rating used by different countries. For example, a rating value can represent a PG-13 rating in the United States and an MA15+ in Australia.

## See Also

### Rating Media Content

var containsExplicitContent: Bool

A Boolean value indicating whether the item contains adult-oriented content.

Deprecated

var contentRatingDomain: TVMediaItem.ContentRatingDomain?

The media domain that the rating applies to.

Deprecated

struct ContentRatingDomain

A value identifying the media’s content rating domain.

Deprecated

