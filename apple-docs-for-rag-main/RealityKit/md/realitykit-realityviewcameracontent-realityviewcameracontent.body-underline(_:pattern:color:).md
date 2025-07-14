

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  underline(\_:pattern:color:) 

Instance Method

# underline(\_:pattern:color:)

Applies an underline to the text in this view.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func underline(
    _ isActive: Bool = true,
    pattern: Text.LineStyle.Pattern = .solid,
    color: Color? = nil
) -> some View
```

## Parameters 

`isActive`  

A Boolean value that indicates whether underline is added. The default value is `true`.

`pattern`  

The pattern of the line. The default value is `solid`.

`color`  

The color of the underline. If `color` is `nil`, the underline uses the default foreground color.

## Return Value

A view where text has a line running along its baseline.

