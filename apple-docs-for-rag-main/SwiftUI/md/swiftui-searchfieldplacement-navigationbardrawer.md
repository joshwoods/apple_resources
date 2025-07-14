

- SwiftUI
- SearchFieldPlacement
-  navigationBarDrawer 

Type Property

# navigationBarDrawer

The search field appears in the navigation bar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let navigationBarDrawer: SearchFieldPlacement
```

## Discussion

The field appears below any navigation bar title and uses the automatic display mode to configure when to hide the search field. To choose a different display mode, use navigationBarDrawer(displayMode:) instead.

## See Also

### Getting a search field placement

static let automatic: SearchFieldPlacement

SwiftUI places the search field automatically.

static func navigationBarDrawer(displayMode: SearchFieldPlacement.NavigationBarDrawerDisplayMode) -> SearchFieldPlacement

The search field appears in the navigation bar using the specified display mode.

static let sidebar: SearchFieldPlacement

The search field appears in the sidebar of a navigation view.

static let toolbar: SearchFieldPlacement

The search field appears in the toolbar.

