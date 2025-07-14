

- Foundation
- Scanner
-  init(string:) 

Initializer

# init(string:)

Returns an `NSScanner` object initialized to scan a given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(string: String)
```

## Parameters 

`string`  

The string to scan.

## Return Value

An `NSScanner` object initialized to scan `aString` from the beginning. The returned object might be different than the original receiver.

## See Also

### Creating a Scanner

class func localizedScanner(with: String) -> Any

Returns an `NSScanner` object that scans a given string according to the user’s default locale.

