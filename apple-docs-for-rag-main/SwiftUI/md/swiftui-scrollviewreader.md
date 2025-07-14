

- SwiftUI
-  ScrollViewReader 

Structure

# ScrollViewReader

A view that provides programmatic scrolling, by working with a proxy to scroll to known child views.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct ScrollViewReader where Content : View
```

## Overview

The scroll view reader’s content view builder receives a ScrollViewProxy instance; you use the proxy’s scrollTo(_:anchor:) to perform scrolling.

The following example creates a ScrollView containing 100 views that together display a color gradient. It also contains two buttons, one each at the top and bottom. The top button tells the ScrollViewProxy to scroll to the bottom button, and vice versa.

```
@Namespace var topID
@Namespace var bottomID

var body: some View {
    ScrollViewReader { proxy in
        ScrollView {
            Button("Scroll to Bottom") {
                withAnimation {
                    proxy.scrollTo(bottomID)
                }
            }
            .id(topID)

            VStack(spacing: 0) {
                ForEach(0.. Color {
    Color(red: fraction, green: 1 - fraction, blue: 0.5)
}
```

Important

You may not use the ScrollViewProxy during execution of the `content` view builder; doing so results in a runtime error. Instead, only actions created within `content` can call the proxy, such as gesture handlers or a view’s `onChange(of:perform:)` method.

## Topics

### Creating a scroll view reader

init(content: (ScrollViewProxy) -> Content)

Creates an instance that can perform programmatic scrolling of its child scroll views.

### Configuring a scroll view reader

var content: (ScrollViewProxy) -> Content

The view builder that creates the reader’s content.

## Relationships

### Conforms To

- View

## See Also

### Creating a scroll view

struct ScrollView

A scrollable view.

struct ScrollViewProxy

A proxy value that supports programmatic scrolling of the scrollable views within a view hierarchy.

