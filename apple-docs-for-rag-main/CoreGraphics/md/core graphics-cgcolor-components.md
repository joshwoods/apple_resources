

- Core Graphics
- CGColor
-  components 

Instance Property

# components

Returns the values of the color components (including alpha) associated with a color.

iOS 7.0+iPadOS 7.0+Mac CatalystmacOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var components: [CGFloat]? { get }
```

## Discussion

An array of intensity values for the color components (including alpha) associated with the specified color. The size of the array is equal to the color’s numberOfComponents value.

## See Also

### Examining a Color

var alpha: CGFloat

Returns the value of the alpha component associated with a color.

var colorSpace: CGColorSpace?

Returns the color space associated with a color.

var numberOfComponents: Int

Returns the number of color components (including alpha) associated with a color.

var pattern: CGPattern?

Returns the pattern associated with a color in a pattern color space.

