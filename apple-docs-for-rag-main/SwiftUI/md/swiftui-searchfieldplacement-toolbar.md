

- SwiftUI
- SearchFieldPlacement
-  toolbar 

Type Property

# toolbar

The search field appears in the toolbar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
static let toolbar: SearchFieldPlacement
```

## Discussion

The precise placement depends on the platform:

- In iOS and watchOS, the search field appears below the navigation bar and is revealed by scrolling.

- In iPadOS, the search field appears in the trailing navigation bar.

- In macOS, the search field appears in the trailing toolbar.

## See Also

### Getting a search field placement

static let automatic: SearchFieldPlacement

SwiftUI places the search field automatically.

static let navigationBarDrawer: SearchFieldPlacement

The search field appears in the navigation bar.

static func navigationBarDrawer(displayMode: SearchFieldPlacement.NavigationBarDrawerDisplayMode) -> SearchFieldPlacement

The search field appears in the navigation bar using the specified display mode.

static let sidebar: SearchFieldPlacement

The search field appears in the sidebar of a navigation view.

