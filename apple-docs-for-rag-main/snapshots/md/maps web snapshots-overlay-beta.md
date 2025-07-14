

- Maps Web Snapshots
-  Overlay Beta

Object

# Overlay

A JSON object for a Snapshot URL that describes overlay shape characteristics, including points for the overlay and styles such as width, color, and dash pattern.

Maps Web Snapshots 1.0+Beta

## Properties

`type`

`string`

An optional property that specifies the type of overlay shape to render.

Default: `”polygon”`

Options: `“circle”, ”polygon”, or “polyline”`

`points`

`*`

An array of coordinates, specified as latitude and longitude coordinate pairs, or as a string encoded with the Encoded Polyline Algorithm Format.

The array format specifies points for a polyline overlay. The following example specifies two points for a polyline overlay as an array of latitude and longitude coordinate pairs:

&quot;points&quot;: [&quot;37.779996,-122.51158&quot;,&quot;37.78040,-122.51348&quot;]

You can provide those same parameters in encoded polyline algorithm format:

&quot;points&quot;: &quot;w{qeFj`wjVwAzJ&quot;

Possible types: `[string]``, ``string`

`center`

`string`

The coordinate of the circle’s center.

`radius`

`number`

The circle’s radius in meters.

`strokeColor`

`string`

The color of the line between each coordinate point. Supported values are HTML color names or hexadecimal color codes.

`lineWidth`

`integer`

The width of the line, in CSS pixels.

`lineDash`

`[integer]`

An array that defines a line’s dash pattern, where numbers represent line and gap lengths in CSS pixels. For example, `[10,5]` means draw a line for 10 pixels, leave a 5-pixel gap, and repeat. An empty array draws a solid line, which is the default.

`fillColor`

`string`

The object’s fill color.

`fillOpacity`

`number`

The opacity value used for filling the object.

`fillRule`

`string`

The rule used to determine the inside of the polygon.

`lineCap`

`string`

The style used for line end points.

Default: `”round”`

Options: `”butt”, “round”, or “square”`

`lineDashOffset`

`integer`

The line dash offset.

`lineGradient`

Overlay.LineGradient

An object that determines color stops for the gradient, positioned by offsets between 0 and 1.

&quot;lineGradient&quot;: {&quot;0&quot;: &quot;green&quot;, &quot;1&quot;: &quot;blue&quot;}

`lineGradientIndexes`

Overlay.LineGradientIndexes

An object that determines where the color stops for the gradient. This property uses indexes of points on the polyline.

&quot;lineGradientIndexes&quot;: {&quot;1&quot;: &quot;blue&quot;}

`lineJoin`

`string`

The style used for joins between line segments.

Default: `“round”`

Options: `“bevel”, “miter”, or “round”`

`strokeOpacity`

`number`

The opacity value for stroking.

`styleIdx`

`integer`

The index number used to reference an `OverlayStyle` object.

## Topics

### Objects

object Overlay.LineGradient

A property that sets the color stops for the gradient, positioned by offsets between 0 and 1.

object Overlay.LineGradientIndexes

A property that sets the color stops for the gradient, positioned by indexes of points on the polyline.

## See Also

### Essentials

Generating a URL and Signature to Create a Maps Web Snapshot

Create a Snapshot URL and generate a signature to validate the request.

object Annotation

An object for a Snapshot URL that describes annotation characteristics.

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

