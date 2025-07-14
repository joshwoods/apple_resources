

- SwiftUI
- View
-  allowedDynamicRange(\_:) 

Instance Method

# allowedDynamicRange(\_:)

Returns a new view configured with the specified allowed dynamic range.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func allowedDynamicRange(_ range: Image.DynamicRange?) -> some View
```

## Parameters 

`range`  

The requested dynamic range, or nil to restore the default allowed range.

## Return Value

A new view.

## Discussion

The following example enables HDR rendering within a view hierarchy:

```
MyView().allowedDynamicRange(.high)
```

## See Also

### Colors and patterns

func backgroundStyle&lt;S>(S) -> some View

Sets the specified style to render backgrounds within the view.

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

