

- SwiftUI
- ContentMarginPlacement
-  scrollIndicators 

Type Property

# scrollIndicators

The scroll indicators placement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var scrollIndicators: ContentMarginPlacement { get }
```

## Discussion

Scrollable views like ScrollView will use this placement to inset their scroll indicators, but not their content.

## See Also

### Getting the placement

static var automatic: ContentMarginPlacement

The automatic placement.

static var scrollContent: ContentMarginPlacement

The scroll content placement.

