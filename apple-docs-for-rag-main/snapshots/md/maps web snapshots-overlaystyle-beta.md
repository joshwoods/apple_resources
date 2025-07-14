

- Maps Web Snapshots
-  OverlayStyle Beta

Object

# OverlayStyle

A JSON object that describes reusable styles for an overlay.

Maps Web Snapshots 1.0+Beta

## Properties

`fillColor`

`string`

The color used to fill the object.

`fillOpacity`

`number`

The opacity value used to fill the object.

`fillRule`

`string`

A rule used to determine the inside space of the polygon.

Default: `“nonzero”`

Options: `“nonzero” or “evenodd”`

`lineCap`

`string`

The style used for line end points.

Default: `“round”`

Options: `”butt”, “round”, or “square”`

`lineDash`

`[integer]`

An array of integers that specifies the line’s dash pattern.

`lineDashOffset`

`integer`

The line dash offset.

`lineGradient`

OverlayStyle.LineGradient

An object that determines color stops for the gradient, positioned by offsets between 0 and 1.

&quot;lineGradient&quot;: {&quot;0&quot;: &quot;green&quot;, &quot;1&quot;: &quot;blue&quot;}

`lineGradientIndexes`

OverlayStyle.LineGradientIndexes

An object that determines where the color stops for the gradient. This property uses indexes of points on the polyline.

&quot;lineGradientIndexes&quot;: {&quot;1&quot;: &quot;blue&quot;}

`lineJoin`

`string`

The style used for joins between line segments.

Options: `”miter”, “round”, or “bevel”`

`lineWidth`

`integer`

An integer in CSS pixels that specifies the width of the line.

`strokeColor`

`string`

The color for stroking.

`strokeOpacity`

`number`

The opacity value for stroking.

## Discussion

You pass the `OverlayStyle` object properties from the `overlayStyles` query parameter. You can set the object properties and reuse the styles for multiple objects. Any changes made to an `OverlayStyle` object property automatically changes the styles associated with that object, unless they’re overwritten using the `Overlay` object.

The following example shows `OverlayStyle` properties passed into the `overlayStyles` query parameter:

/snapshot?center=0,0&amp;z=7&amp;overlays=[{
&quot;type&quot;: &quot;polygon&quot;,
&quot;points&quot;:[&quot;1,1&quot;,&quot;1,-1&quot;,&quot;-1,-1&quot;,&quot;-1,1&quot;],
&quot;styleIdx&quot;: 2
}]
&amp;overlayStyles=[{
&quot;fillColor&quot;: &quot;teal&quot;,
&quot;fillOpacity&quot;: 0.7,
&quot;strokeColor&quot;: &quot;blue&quot;,
&quot;lineCap&quot;: &quot;square&quot;,
&quot;lineWidth&quot;: 11,
&quot;strokeOpacity&quot;: 0.7 }]

## Topics

### Objects

object OverlayStyle.LineGradient

A property that sets the color stops for the gradient, positioned by offsets between 0 and 1.

object OverlayStyle.LineGradientIndexes

A property that sets the color stops for the gradient, positioned by indexes of points on the polyline.

## See Also

### Essentials

Generating a URL and Signature to Create a Maps Web Snapshot

Create a Snapshot URL and generate a signature to validate the request.

object Annotation

An object for a Snapshot URL that describes annotation characteristics.

Beta

object Overlay

A JSON object for a Snapshot URL that describes overlay shape characteristics, including points for the overlay and styles such as width, color, and dash pattern.

Beta

object Image

A JSON object for a Snapshot URL that describes the characteristics of custom images to use for map annotations.

Beta

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software 

