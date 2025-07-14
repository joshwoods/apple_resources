

- UIKit
- UIPrintInfo
-  init(coder:) 

Initializer

# init(coder:)

Creates a print info object from data in an unarchiver.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating a print info object

class func printInfo() -> UIPrintInfo

Returns a print-information object initialized with default values.

init(dictionary: [AnyHashable : Any]?)

Returns a print-information object that is initialized with the data in the passed-in dictionary.

var dictionaryRepresentation: [AnyHashable : Any]

A dictionary representation of a print-information object.

