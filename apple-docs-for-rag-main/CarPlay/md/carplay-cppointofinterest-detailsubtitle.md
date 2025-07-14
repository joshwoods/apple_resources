

- CarPlay
- CPPointOfInterest
-  detailSubtitle 

Instance Property

# detailSubtitle

The detail card’s subtitle.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var detailSubtitle: String? { get set }
```

## Discussion

The template only displays a detail card when the user selects a point of interest. If this property is nil, the card displays the point of interest’s subtitle instead.

## See Also

### Managing the Detail Card’s Data

var detailTitle: String?

The detail card’s title.

var detailSummary: String?

The detail card’s summary.

