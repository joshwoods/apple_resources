

- UIKit
- UIPrintInfo
-  printInfo() 

Type Method

# printInfo()

Returns a print-information object initialized with default values.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func printInfo() -> UIPrintInfo
```

## Return Value

An instance of `UIPrintInfo` or `nil` if the object could not be created.

## See Also

### Creating a print info object

init(dictionary: [AnyHashable : Any]?)

Returns a print-information object that is initialized with the data in the passed-in dictionary.

var dictionaryRepresentation: [AnyHashable : Any]

A dictionary representation of a print-information object.

init?(coder: NSCoder)

Creates a print info object from data in an unarchiver.

