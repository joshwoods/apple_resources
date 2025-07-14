

- Device Management
-  Artwork 

Object

# Artwork

An object that represents artwork.

Device Assignment ServicesVPP License Management

``` source
object Artwork
```

## Properties

`assetToken`

`string`

`bgColor`

`string`

The average background color for the image to use as a placeholder.

`gradient`

Artwork.Gradient

Gradient information. If absent, use existing gradient behavior. If present, but the body is an empty object {}, then gradient is disabled. This overrides any setting in the editorial item.

`hasP3`

`boolean`

`height`

`number`

 (Required) 

The largest height available for the source image.

`pictureFileType`

`string`

`supportsLayeredImage`

`boolean`

`textColor1`

`string`

A primary text color appropriate to use with the artwork.

`textColor2`

`string`

A secondary text color appropriate to use with the artwork.

`textColor3`

`string`

An auxiliary text color appropriate to use with the artwork.

`textColor4`

`string`

An auxiliary text color appropriate to use with the artwork.

`url`

`string`

 (Required) 

The URL of the image. May be templated to allow customizing the height {h}, width {w}, and crop code {c}.

`width`

`number`

 (Required) 

The largest width available for the source image.

## Topics

### Related Objects

object Artwork.Gradient

An object that represents the properties of a color gradient for an artwork object.

## See Also

### Getting common type information

object DescriptionAttribute

An object that represents a description attribute.

object Genres

A resource object that represents a music genre.

object Apps

A resource object that represents an app.

object Books

A resource object that represents a book.

