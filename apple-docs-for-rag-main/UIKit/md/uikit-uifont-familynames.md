

- UIKit
- UIFont
-  familyNames 

Type Property

# familyNames

Returns an array of font family names available on the system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class var familyNames: [String] { get }
```

## Return Value

An array of `NSString` objects, each of which contains the name of a font family.

## Discussion

Font family names correspond to the base name of a font, such as `Times New Roman`. You can pass the returned strings to the fontNames(forFamilyName:) method to retrieve a list of font names available for that family. You can then use the corresponding font name to retrieve an actual font object.

## See Also

### Getting the Available Font Names

class func fontNames(forFamilyName: String) -> [String]

Returns an array of font names available in a particular font family.

