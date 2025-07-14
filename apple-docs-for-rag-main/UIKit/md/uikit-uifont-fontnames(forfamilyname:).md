

- UIKit
- UIFont
-  fontNames(forFamilyName:) 

Type Method

# fontNames(forFamilyName:)

Returns an array of font names available in a particular font family.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func fontNames(forFamilyName familyName: String) -> [String]
```

## Parameters 

`familyName`  

The name of the font family. Use the familyNames method to get an array of the available font family names on the system.

## Return Value

An array of `NSString` objects, each of which contains a font name associated with the specified family.

## Discussion

You can pass the returned strings as parameters to the init(name:size:) method to retrieve an actual font object.

## See Also

### Related Documentation

init?(name: String, size: CGFloat)

Creates and returns a font object for the specified font name and size.

### Getting the Available Font Names

class var familyNames: [String]

Returns an array of font family names available on the system.

