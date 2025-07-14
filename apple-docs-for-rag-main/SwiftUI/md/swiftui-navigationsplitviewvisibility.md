

- SwiftUI
-  NavigationSplitViewVisibility 

Structure

# NavigationSplitViewVisibility

The visibility of the leading columns in a navigation split view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct NavigationSplitViewVisibility
```

## Overview

Use a value of this type to control the visibility of the columns of a NavigationSplitView. Create a State property with a value of this type, and pass a Binding to that state to the init(columnVisibility:sidebar:detail:) or init(columnVisibility:sidebar:content:detail:) initializer when you create the navigation split view. You can then modify the value elsewhere in your code to:

- Hide all but the trailing column with detailOnly.

- Hide the leading column of a three-column navigation split view with doubleColumn.

- Show all the columns with all.

- Rely on the automatic behavior for the current context with automatic.

Note

Some platforms don’t respect every option. For example, macOS always displays the content column.

## Topics

### Getting visibilities

static var automatic: NavigationSplitViewVisibility

Use the default leading column visibility for the current device.

static var all: NavigationSplitViewVisibility

Show all the columns of a three-column navigation split view.

static var doubleColumn: NavigationSplitViewVisibility

Show the content column and detail area of a three-column navigation split view, or the sidebar column and detail area of a two-column navigation split view.

static var detailOnly: NavigationSplitViewVisibility

Hide the leading two columns of a three-column navigation split view, so that just the detail area shows.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Presenting views in columns

Bringing robust navigation structure to your SwiftUI app

Use navigation links, stacks, destinations, and paths to provide a streamlined experience for all platforms, as well as behaviors such as deep linking and state restoration.

Migrating to new navigation types

Improve navigation behavior in your app by replacing navigation views with navigation stacks and navigation split views.

struct NavigationSplitView

A view that presents views in two or three columns, where selections in leading columns control presentations in subsequent columns.

func navigationSplitViewStyle&lt;S>(S) -> some View

Sets the style for navigation split views within this view.

func navigationSplitViewColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the column containing this view.

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

struct NavigationLink

A view that controls a navigation presentation.

