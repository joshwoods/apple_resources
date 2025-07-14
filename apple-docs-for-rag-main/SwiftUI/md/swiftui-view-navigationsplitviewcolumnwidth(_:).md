

- SwiftUI
- View
-  navigationSplitViewColumnWidth(\_:) 

Instance Method

# navigationSplitViewColumnWidth(\_:)

Sets a fixed, preferred width for the column containing this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func navigationSplitViewColumnWidth(_ width: CGFloat) -> some View
```

## Discussion

Apply this modifier to the content of a column in a NavigationSplitView to specify a fixed preferred width for the column. Use navigationSplitViewColumnWidth(min:ideal:max:) if you need to specify a flexible width.

The following example shows a three-column navigation split view where the first column has a preferred width of 150 points, and the second column has a flexible, preferred width between 150 and 400 points:

```
NavigationSplitView {
    MySidebar()
        .navigationSplitViewColumnWidth(150)
} contents: {
    MyContents()
        .navigationSplitViewColumnWidth(
            min: 150, ideal: 200, max: 400)
} detail: {
    MyDetail()
}
```

Only some platforms enable resizing columns. If you specify a width that the current presentation environment doesn’t support, SwiftUI may use a different width for your column.

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

func navigationSplitViewColumnWidth(min: CGFloat?, ideal: CGFloat, max: CGFloat?) -> some View

Sets a flexible, preferred width for the column containing this view.

struct NavigationSplitViewVisibility

The visibility of the leading columns in a navigation split view.

struct NavigationLink

A view that controls a navigation presentation.

