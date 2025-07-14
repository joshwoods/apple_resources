

- UIKit
- UIPasteConfiguration
-  init(acceptableTypeIdentifiers:) 

Initializer

# init(acceptableTypeIdentifiers:)

Initializes a new paste configuration with a specified array of acceptable UTIs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(acceptableTypeIdentifiers: [String])
```

## Parameters 

`acceptableTypeIdentifiers`  

An array of uniform type identifier (UTI) strings.

## Return Value

A paste configuration that is initialized with the specified UTI strings.

## Discussion

Specify the acceptable UTIs in descending order of fidelity. The UTI that provides the richest data representation should be first in the list. For instance, if the data to paste is contact information, list the vCard UTI first, followed by the plain text UTI.

## See Also

### Initializing a paste configuration

init()

Initializes a new paste configuration.

convenience init(forAccepting: any NSItemProviderReading.Type)

Initializes a new paste configuration with the UTIs declared as supported by a specified class.

convenience init&lt;T>(forAccepting: T.Type)

