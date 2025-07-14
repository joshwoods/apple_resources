

- UIKit
- UIPrintInteractionController
-  canPrint(\_:) 

Type Method

# canPrint(\_:)

Returns a Boolean value that indicates whether UIKit can print the file that the specified URL references.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func canPrint(_ url: URL) -> Bool
```

## Parameters 

`url`  

An object representing a URL. Valid `NSURL` objects must use the `file:` or any scheme that can return an NSData object with a registered protocol. The file referenced by the URL must contain PDF data or an image in a format supported by the Image I/O framework. See View Programming Guide for iOS in View Programming Guide for iOS for a list of the supported image formats.

## Return Value

true if UIKit can print the contents of the referenced file, otherwise false. The method returns false if `url` references PDF data that specifies that printing is not allowed.

## Discussion

You should call this method to test the data referenced by a URL prior to assigning that URL to printingItem or printingItems.

## See Also

### Determining printability

class var isPrintingAvailable: Bool

A Boolean value that indicates whether the device supports printing.

class func canPrint(Data) -> Bool

Returns a Boolean value that indicates whether UIKit can print the contents of a data object.

class var printableUTIs: Set&lt;String>

Returns a set of the Uniform Type Identifiers for the types of data that UIKit can print.

