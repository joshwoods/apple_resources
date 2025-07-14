

- SwiftUI
-  SearchFieldPlacement 

Structure

# SearchFieldPlacement

The placement of a search field in a view hierarchy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SearchFieldPlacement
```

## Mentioned in 

Adding a search interface to your app

## Overview

You can give a preferred placement to any of the searchable modifiers, like searchable(text:placement:prompt:):

```
var body: some View {
    NavigationView {
        PrimaryView()
        SecondaryView()
        Text("Select a primary and secondary item")
    }
    .searchable(text: $text, placement: .sidebar)
}
```

Depending on the containing view hierachy, SwiftUI might not be able to fulfill your request.

## Topics

### Getting a search field placement

static let automatic: SearchFieldPlacement

SwiftUI places the search field automatically.

static let navigationBarDrawer: SearchFieldPlacement

The search field appears in the navigation bar.

static func navigationBarDrawer(displayMode: SearchFieldPlacement.NavigationBarDrawerDisplayMode) -> SearchFieldPlacement

The search field appears in the navigation bar using the specified display mode.

static let sidebar: SearchFieldPlacement

The search field appears in the sidebar of a navigation view.

static let toolbar: SearchFieldPlacement

The search field appears in the toolbar.

### Supporting types

struct NavigationBarDrawerDisplayMode

A mode that determines when to display a search field that appears in a navigation bar.

## Relationships

### Conforms To

- Sendable

## See Also

### Searching your app’s data model

Adding a search interface to your app

Present an interface that people can use to search for content in your app.

Performing a search operation

Update search results based on search text and optional tokens that you store.

func searchable(text:placement:prompt:)

Marks this view as searchable, which configures the display of a search field.

func searchable(text:tokens:placement:prompt:token:)

Marks this view as searchable with text and tokens.

func searchable(text:editableTokens:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

