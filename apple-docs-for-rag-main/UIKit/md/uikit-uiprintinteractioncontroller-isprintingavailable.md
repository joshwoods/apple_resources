

- UIKit
- UIPrintInteractionController
-  isPrintingAvailable 

Type Property

# isPrintingAvailable

A Boolean value that indicates whether the device supports printing.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class var isPrintingAvailable: Bool { get }
```

## Discussion

This value is true if the device supports printing, otherwise false. An application can show or hide any print buttons based on this value.

## See Also

### Determining printability

class func canPrint(Data) -> Bool

Returns a Boolean value that indicates whether UIKit can print the contents of a data object.

class func canPrint(URL) -> Bool

Returns a Boolean value that indicates whether UIKit can print the file that the specified URL references.

class var printableUTIs: Set&lt;String>

Returns a set of the Uniform Type Identifiers for the types of data that UIKit can print.

