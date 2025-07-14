

- SwiftUI
- ContentMarginPlacement
-  scrollContent 

Type Property

# scrollContent

The scroll content placement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var scrollContent: ContentMarginPlacement { get }
```

## Discussion

Scrollable views like ScrollView will use this placement to inset their content, but not their scroll indicators.

## See Also

### Getting the placement

static var automatic: ContentMarginPlacement

The automatic placement.

static var scrollIndicators: ContentMarginPlacement

The scroll indicators placement.

