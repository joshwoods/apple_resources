

- Foundation
- NSCharacterSet
-  init(contentsOfFile:) 

Initializer

# init(contentsOfFile:)

Returns a character set read from the bitmap representation stored in the file a given path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(contentsOfFile fName: String)
```

## Parameters 

`fName`  

A path to a file containing a bitmap representation of a character set. The path name must end with the extension `.bitmap`.

## Return Value

A character set read from the bitmap representation stored in the file at `path`.

## Discussion

This method doesn’t use filenames to check for the uniqueness of the character sets it creates. To prevent duplication of character sets in memory, cache them and make them available through an API that checks whether the requested set has already been loaded.

To read a bitmap representation from any file, use the `NSData` methoddataWithContentsOfFile:options:error: and pass the result to init(bitmapRepresentation:).

## See Also

### Creating and Managing Character Sets as Bitmap Representations

init(bitmapRepresentation: Data)

Returns a character set containing characters determined by a given bitmap representation.

var bitmapRepresentation: Data

An `NSData` object encoding the receiver in binary format.

