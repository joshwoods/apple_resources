

- Foundation
- Scanner
-  localizedScanner(with:) 

Type Method

# localizedScanner(with:)

Returns an `NSScanner` object that scans a given string according to the user’s default locale.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func localizedScanner(with string: String) -> Any
```

## Parameters 

`string`  

The string to scan.

## Return Value

An `NSScanner` object that scans `aString` according to the user’s default locale.

## Discussion

Sets the string to scan by invoking init(string:) with `aString`. The locale is set with Scanner.

## See Also

### Creating a Scanner

init(string: String)

Returns an `NSScanner` object initialized to scan a given string.

