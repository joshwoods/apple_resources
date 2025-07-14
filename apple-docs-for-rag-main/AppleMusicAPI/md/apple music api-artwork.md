

- Apple Music API
-  Artwork 

Object

# Artwork

An object that represents artwork.

Apple Music 1.0+

``` source
object Artwork
```

## Properties

`bgColor`

`string`

The average background color of the image.

`height`

`number`

 (Required) 

The maximum height available for the image.

`width`

`number`

 (Required) 

The maximum width available for the image.

`textColor1`

`string`

The primary text color used if the background color gets displayed.

`textColor2`

`string`

The secondary text color used if the background color gets displayed.

`textColor3`

`string`

The tertiary text color used if the background color gets displayed.

`textColor4`

`string`

The final post-tertiary text color used if the background color gets displayed.

`url`

`string`

 (Required) 

The URL to request the image asset. `{w}x{h}`must precede image filename, as placeholders for the `width` and `height` values as described above. For example, `{w}x{h}bb.jpeg`).

