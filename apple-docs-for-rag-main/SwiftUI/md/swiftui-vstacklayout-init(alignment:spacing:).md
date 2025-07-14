

- SwiftUI
- VStackLayout
-  init(alignment:spacing:) 

Initializer

# init(alignment:spacing:)

Creates a vertical stack with the specified spacing and horizontal alignment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    alignment: HorizontalAlignment = .center,
    spacing: CGFloat? = nil
)
```

## Parameters 

`alignment`  

The guide for aligning the subviews in this stack. It has the same horizontal screen coordinate for all subviews.

`spacing`  

The distance between adjacent subviews. Set this value to `nil` to use default distances between subviews.

