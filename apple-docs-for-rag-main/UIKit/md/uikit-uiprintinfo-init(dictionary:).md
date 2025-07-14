

- UIKit
- UIPrintInfo
-  init(dictionary:) 

Initializer

# init(dictionary:)

Returns a print-information object that is initialized with the data in the passed-in dictionary.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(dictionary: [AnyHashable : Any]?)
```

## Parameters 

`dictionary`  

A dictionary that contains data to initialize the `UIPrintInfo` object with.

## Return Value

An instance of `UIPrintInfo` or `nil` if the object could not be created.

## Discussion

You use the `dictionary` parameter to initialize a `UIPrintInfo` object with stored print-job information. Some applications might archive a previous `UIPrintInfo` object and use that for a future print job with this method.

You can later access the dictionary by calling the dictionaryRepresentation method on the `UIPrintInfo` object.

## See Also

### Creating a print info object

class func printInfo() -> UIPrintInfo

Returns a print-information object initialized with default values.

var dictionaryRepresentation: [AnyHashable : Any]

A dictionary representation of a print-information object.

init?(coder: NSCoder)

Creates a print info object from data in an unarchiver.

