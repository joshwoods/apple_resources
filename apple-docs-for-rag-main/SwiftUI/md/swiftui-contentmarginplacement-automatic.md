

- SwiftUI
- ContentMarginPlacement
-  automatic 

Type Property

# automatic

The automatic placement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var automatic: ContentMarginPlacement { get }
```

## Discussion

Views that support margin customization can automatically use margins with this placement. For example, a ScrollView will use this placement to automatically inset both its content and scroll indicators by the specified amount.

## See Also

### Getting the placement

static var scrollContent: ContentMarginPlacement

The scroll content placement.

static var scrollIndicators: ContentMarginPlacement

The scroll indicators placement.

