

- CarPlay
- CPPointOfInterest
-  detailTitle 

Instance Property

# detailTitle

The detail card’s title.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var detailTitle: String? { get set }
```

## Discussion

The template only displays the detail card when a user selects a point of interest. If this property is nil, the card displays the point of interest’s title instead.

## See Also

### Managing the Detail Card’s Data

var detailSubtitle: String?

The detail card’s subtitle.

var detailSummary: String?

The detail card’s summary.

