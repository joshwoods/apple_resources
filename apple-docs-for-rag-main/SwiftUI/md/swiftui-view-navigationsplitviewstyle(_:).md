

- SwiftUI
- View
-  navigationSplitViewStyle(\_:) 

Instance Method

# navigationSplitViewStyle(\_:)

Sets the style for navigation split views within this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func navigationSplitViewStyle(_ style: S) -> some View where S : NavigationSplitViewStyle
```

## Parameters 

`style`  

The style to set.

## Return Value

A view that uses the specified navigation split view style.

## Mentioned in 

Migrating to new navigation types

## See Also

### Presenting views in columns

Bringing robust navigation structure to your SwiftUI app

Use navigation links, stacks, destinations, and paths to provide a streamlined experience for all platforms, as well as behaviors such as deep linking and state restoration.

Migrating to new navigation types

Improve navigation behavior in your app by replacing navigation views with navigation stacks and navigation split views.

struct NavigationSplitView

A view that presents views in two or three columns, where selections in leading columns control presentations in subsequent columns.

func navigationSplitViewColumnWidth(CGFloat) -> some View

Sets a fixed, preferred width for the column containing this view.

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

struct NavigationSplitViewVisibility

The visibility of the leading columns in a navigation split view.

struct NavigationLink

A view that controls a navigation presentation.

