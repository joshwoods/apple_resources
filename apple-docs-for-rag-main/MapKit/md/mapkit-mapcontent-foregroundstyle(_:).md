

- MapKit
- MapContent
-  foregroundStyle(\_:) 

Instance Method

# foregroundStyle(\_:)

Specifies the shape style used to fill content in drawing map overlays.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func foregroundStyle(_ content: some ShapeStyle) -> some MapContent
```

## Parameters 

`content`  

The shape style to apply to the overlay.

## Return Value

Returns MapContent with the foreground style you specified.

## See Also

### Setting the content style

func tint&lt;S>(S) -> some MapContent

The tint shape style to apply to map content.

