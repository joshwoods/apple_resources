

- Maps Web Snapshots
-  Create a Maps Web Snapshot Beta

Web Service Endpoint

# Create a Maps Web Snapshot

Generates a map image with characteristics that you provide in the query parameters.

Maps Web Snapshots 1.0+Beta

## URL

``` source
GET https://snapshot.apple-mapkit.com/api/v1/snapshot
```

## Query Parameters

`teamId`

`string`

**Only use this parameter if you don’t provide a token parameter.** Your Apple Developer Team ID. For more information, see Creating a Maps identifier and a private key.

`keyId`

`string`

**Only use this parameter if you don’t provide a token parameter.** Your MapKit JS Key ID. For more information, see Creating a Maps identifier and a private key.

`signature`

`string`

**Only use this parameter if you don’t provide a token parameter.** A Base64, URL-encoded signature that signs the request path and query parameters. The signature must be the last parameter in the request URL; otherwise, the request returns status code `401 Unauthorized`. See Generating a URL and Signature to Create a Maps Web Snapshot.

`center`

`string`

 (Required) 

The center of the map. You can specify `center` as coordinates, as an address, or with the string `auto` when you add annotations and overlays.

Provide coordinates as a string with the latitude and longitude separated by a comma, such as:

center=&quot;37.78,-122.42&quot;

If you specify `center` as coordinates, the latitude must be in the range `(-90, 90)` and longitude must be in the range `(-180, 180)`.

A geocoded address is a valid value for the `center` parameter, such as:

center=&quot;1 Apple Park Way in Cupertino, California&quot;

The string `auto` is also a valid value for the `center` parameter, for example:

center=&quot;auto&quot;

If you specify `center=”auto”`, the Web Map Snapshot API returns a map that includes all overlays or annotations. The API requires `annotations` or `overlays` when you use `center=”auto”`.

`z`

`float`

The zoom level of the map.

The Web Map Snapshot API ignores the `z` parameter when you specify `auto` for the `center` parameter, or when you specify both `spn` and `z` parameters.

Default: `12`

Minimum Value: `3`

Maximum Value: `20`

`spn`

`string`

A comma-separated coordinate span that indicates how much of the map Web Map Snapshots API displays around the map’s center. The latitude must be in the range of `(0, 90)`, and the longitude must be in the range `(0, 180)`. The latitude and longitude delta parameters must be positive numbers; the API treats negative numbers as `0`.

The Web Map Snapshot API ignores the `spn` parameter if you specify `auto` for the `center` parameter. If you provide both `z` and `spn` parameters, the value for `spn` takes precedence over `z`.

`size`

`string`

The size of the image in pixels. Specify the `size` as width and height integers separated by the character `x`. For example, `640x480` creates an image 640 pixels wide and 480 pixels tall.

The width and height must be within the range of `[50, 640]`.

Default: `600x400`

`scale`

`int32`

The pixel density of the image. `scale=2` returns an image intended for 2x Retina displays. Setting `scale` to values greater than `1` increases the number of pixels in the generated image.

Default: `1`

Minimum Value: `1`

Maximum Value: `3`

Possible Values: `1, 2, 3`

`t`

`string`

The map type.

Default: `standard`

Possible Values: `standard, hybrid, satellite, mutedStandard`

`colorScheme`

`string`

The color scheme of the map. The `dark` color scheme only applies to the `standard` and `mutedStandard` map types.

Default: `light`

Possible Values: `light, dark`

`poi`

`boolean`

A Boolean value that indicates whether to show points of interest on the map. To hide points of interest, set `poi=0`.

Default: `1`

`lang`

`string`

The language that Maps Web Snapshots API uses for labels on the map. Supported values are locale IDs, such as `en-GB` or `es-MX`.

Default: `en-US`

`annotations`

`[`Annotation`]`

An array of annotations to display on the map, which you specify as JSON Annotation objects. Annotations layer on top of the map in the order you specify in the request.

`overlays`

`[`Overlay`]`

An array of overlays to display on the map, which you specify as an array of JSON Overlay objects.

`overlayStyles`

`[`OverlayStyle`]`

A JSON array of overlay styles. This object allows you to reuse style values on different overlays.

`imgs`

`[`Image`]`

An array of custom images to annotate the map, specified as an array of JSON Image objects.

`referer`

`string`

**Only use this parameter if you don’t provide a token parameter.** The `referer` string value to match against the request’s `Referer` header value. Requests that don’t match the `referer` parameter fail with HTTP status code `401 Unauthorized`. Set a referrer restriction through the `referer` parameter.

`expires`

`int64`

**Only use this parameter if you don’t provide a token parameter.** The time in seconds from epoch at which the request expires. Expired requests fail with HTTP status code `401 Unauthorized`. Set an expiration through the `expires` parameter.

`token`

`string`

A developer’s Maps token. For information on how to create a Maps token, see Creating a Maps token.

## Response Codes

` 200 ``OK`

`binary`

`OK`

The request was successful and the Maps Web Snapshots API returned a map image as `image/png`.

Content-Type: image/png

` 400 ``Bad Request`

`Bad Request`

The request is invalid.

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

This request contains invalid authorization credentials.

Content-Type: application/json

` 413 ``Request Entity Too Large`

`Request Entity Too Large`

The URL for this request exceeds the maximum number of characters allowed.

Content-Type: application/json

` 429 `

You exceeded the rate limit for your API key. You need to wait and try the request again.

Content-Type: application/json

` 500 ``Internal Server Error`

`Internal Server Error`

The request failed. This may be due to a temporary outage. Check the Apple Developer System Status Page for up-to-date information on the Web Map Snapshot API.

Content-Type: application/json

## Discussion

Use the Snapshot URL query parameters to define characteristics of the map image such as dimensions, language, color scheme, and more.

You must sign every Snapshot URL request and include the signature as the final parameter. For details and example code, see Generating a URL and Signature to Create a Maps Web Snapshot.

Beta Software

This documentation contains preliminary information about an API or technology in development. This information is subject to change, and software implemented according to this documentation should be tested with final operating system software.

Learn more about using Apple's beta software 

