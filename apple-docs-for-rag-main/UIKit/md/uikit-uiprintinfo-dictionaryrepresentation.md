

- UIKit
- UIPrintInfo
-  dictionaryRepresentation 

Instance Property

# dictionaryRepresentation

A dictionary representation of a print-information object.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var dictionaryRepresentation: [AnyHashable : Any] { get }
```

## Return Value

A dictionary representation of a `UIPrintInfo` object that can be archived and used to create a new `UIPrintInfo` object. Returns `nil` if no dictionary can be created.

## See Also

### Creating a print info object

class func printInfo() -> UIPrintInfo

Returns a print-information object initialized with default values.

init(dictionary: [AnyHashable : Any]?)

Returns a print-information object that is initialized with the data in the passed-in dictionary.

init?(coder: NSCoder)

Creates a print info object from data in an unarchiver.

