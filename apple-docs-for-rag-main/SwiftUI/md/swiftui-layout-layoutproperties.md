

- SwiftUI
- Layout
-  layoutProperties 

Type Property

# layoutProperties

Properties of a layout container.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var layoutProperties: LayoutProperties { get }
```

**Required** Default implementation provided.

## Discussion

Implement this property in a type that conforms to the Layout protocol to characterize your custom layout container. For example, you can indicate that your layout has a vertical stackOrientation:

```
extension BasicVStack {
    static var layoutProperties: LayoutProperties {
        var properties = LayoutProperties()
        properties.stackOrientation = .vertical
        return properties
    }
}
```

If you don’t implement this property in your custom layout, the protocol provides a default implementation, namely layoutProperties, that returns a LayoutProperties instance with default values.

## Default Implementations

### Layout Implementations

static var layoutProperties: LayoutProperties

The default property values for a layout.

## See Also

### Reporting layout container characteristics

func explicitAlignment(of:in:proposal:subviews:cache:)

Returns the position of the specified horizontal alignment guide along the x axis.

**Required** Default implementations provided.

func spacing(subviews: Self.Subviews, cache: inout Self.Cache) -> ViewSpacing

Returns the preferred spacing values of the composite view.

**Required** Default implementation provided.

