

- UIKit
- UIPrintInteractionController
-  printableUTIs 

Type Property

# printableUTIs

Returns a set of the Uniform Type Identifiers for the types of data that UIKit can print.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class var printableUTIs: Set { get }
```

## Return Value

A set object that contains, as strings, the UTIs identifying data types that UIKit knows how to print natively.

## See Also

### Determining printability

class var isPrintingAvailable: Bool

A Boolean value that indicates whether the device supports printing.

class func canPrint(Data) -> Bool

Returns a Boolean value that indicates whether UIKit can print the contents of a data object.

class func canPrint(URL) -> Bool

Returns a Boolean value that indicates whether UIKit can print the file that the specified URL references.

