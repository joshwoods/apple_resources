

- TVMLKit
- TVMediaItem
-  containsExplicitContent Deprecated

Instance Property

# containsExplicitContent

A Boolean value indicating whether the item contains adult-oriented content.

tvOS 12.0–18.0Deprecated

``` source
var containsExplicitContent: Bool { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

This property is ignored when the type is `video`.

## See Also

### Rating Media Content

var contentRatingDomain: TVMediaItem.ContentRatingDomain?

The media domain that the rating applies to.

Deprecated

struct ContentRatingDomain

A value identifying the media’s content rating domain.

Deprecated

var contentRatingRanking: NSNumber?

The rating for a video item.

Deprecated

