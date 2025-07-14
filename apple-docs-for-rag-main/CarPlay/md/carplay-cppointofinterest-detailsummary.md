

- CarPlay
- CPPointOfInterest
-  detailSummary 

Instance Property

# detailSummary

The detail card’s summary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var detailSummary: String? { get set }
```

## Discussion

The template only displays a detail card when the user selects a point of interest. If this property is nil, the card displays the point of interest’s summary instead.

## See Also

### Managing the Detail Card’s Data

var detailTitle: String?

The detail card’s title.

var detailSubtitle: String?

The detail card’s subtitle.

