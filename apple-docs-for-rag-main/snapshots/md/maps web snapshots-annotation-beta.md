

- Maps Web Snapshots
-  Annotation Beta

Object

# Annotation

An object for a Snapshot URL that describes annotation characteristics.

Maps Web Snapshots 1.0+Beta

## Properties

`markerStyle`

`string`

The style of the annotation. Supported styles include `do`t, `balloon`, `large`, and `img`. If you use `img`, you must also specify `imgIdx`, and may specify `offset`.

Default: `balloon`

Possible Values: `dot, balloon, large, img`

`point`

`string`

A single point that defines the location at which to place an annotation. Supported values include latitude and longitude coordinates, addresses, or the keyword `center`, which places an annotation on the map’s center point.

`color`

`string`

The color of the annotation. Supported values are HTML color names or hexadecimal color codes. For example:

annotations=[{&quot;point&quot;:&quot;37.78,-122.42&quot;, &quot;color&quot;:&quot;449944&quot;}]

If the annotation has an “`img`” `markerStyle`, the Maps Web Snapshots API ignores this parameter.

`glyphColor`

`string`

The tint color of the glyph. This property accepts a color name or a hexadecimal color value.

`glyphImgIdx`

`integer`

The zero-based index of the glyph image referenced in the array of images used for a specific annotation.

Don’t set the` glyphText `property when using this property. If the annotation has a `“dot”` or `“img”` `markerStyle`, the Maps Web Snapshots API ignores this parameter.

`glyphText`

`string`

A single alphanumeric character from the set {`a`-`z`, `A`-`Z`, `0`-`9`}, displayed inside the annotation. If the annotation has a “`dot`” or “`img`” `markerStyle`, the Maps Web Snapshots API ignores this parameter.

`imgIdx`

`integer`

The zero-based index of the image referenced in the array of images to use for this annotation. The Maps Web Snapshots API requires this property if `markerStyle` is `img`.

`offset`

`string`

An optional offset in scale independent pixels of the image from the bottom center. Specify the offset as a comma-separated string with x and y values. X values move the element to the left or right with positive and negative values, respectively. Y values move the element up or down with positive and negative values, respectively. For example, the following value moves the element down 5 scale-independent pixels:

The Maps Web Snapshots API ignores the offset property if `markerStyle` is `dot`, `balloon`, or `large`.

## See Also

### Essentials

Generating a URL and Signature to Create a Maps Web Snapshot

Create a Snapshot URL and generate a signature to validate the request.

object Overlay

A JSON object for a Snapshot URL that describes overlay shape characteristics, including points for the overlay and styles such as width, color, and dash pattern.

Beta

object OverlayStyle

A JSON object that describes reusable styles for an overlay.

Beta

object Image

A JSON object for a Snapshot URL that describes the characteristics of custom images to use for map annotations.

Beta

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software 

