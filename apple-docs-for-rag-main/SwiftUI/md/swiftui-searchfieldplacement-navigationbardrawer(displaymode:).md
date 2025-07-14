

- SwiftUI
- SearchFieldPlacement
-  navigationBarDrawer(displayMode:) 

Type Method

# navigationBarDrawer(displayMode:)

The search field appears in the navigation bar using the specified display mode.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
static func navigationBarDrawer(displayMode: SearchFieldPlacement.NavigationBarDrawerDisplayMode) -> SearchFieldPlacement
```

## Parameters 

`displayMode`  

A control that indicates whether to hide the search field in response to scrolling.

## Discussion

The field appears below any navigation bar title. The system can hide the field in response to scrolling, depending on the `displayMode` that you set.

## See Also

### Getting a search field placement

static let automatic: SearchFieldPlacement

SwiftUI places the search field automatically.

static let navigationBarDrawer: SearchFieldPlacement

The search field appears in the navigation bar.

static let sidebar: SearchFieldPlacement

The search field appears in the sidebar of a navigation view.

static let toolbar: SearchFieldPlacement

The search field appears in the toolbar.

