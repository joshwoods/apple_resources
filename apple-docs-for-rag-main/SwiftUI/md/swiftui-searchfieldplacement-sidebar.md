

- SwiftUI
- SearchFieldPlacement
-  sidebar 

Type Property

# sidebar

The search field appears in the sidebar of a navigation view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static let sidebar: SearchFieldPlacement
```

## Mentioned in 

Adding a search interface to your app

## Discussion

The precise placement depends on the platform:

- In iOS and iPadOS the search field appears in the section of the navigation bar associated with the sidebar.

- In macOS, the search field appears inline with the sidebar’s content.

If a sidebar isn’t available, like when you apply the searchable modifier to a view other than a navigation split view, SwiftUI uses automatic placement instead.

## See Also

### Getting a search field placement

static let automatic: SearchFieldPlacement

SwiftUI places the search field automatically.

static let navigationBarDrawer: SearchFieldPlacement

The search field appears in the navigation bar.

static func navigationBarDrawer(displayMode: SearchFieldPlacement.NavigationBarDrawerDisplayMode) -> SearchFieldPlacement

The search field appears in the navigation bar using the specified display mode.

static let toolbar: SearchFieldPlacement

The search field appears in the toolbar.

