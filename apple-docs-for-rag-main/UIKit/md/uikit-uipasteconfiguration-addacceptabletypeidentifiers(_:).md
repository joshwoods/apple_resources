

- UIKit
- UIPasteConfiguration
-  addAcceptableTypeIdentifiers(\_:) 

Instance Method

# addAcceptableTypeIdentifiers(\_:)

Adds an array of UTI strings to a paste configuration, increasing the variety of types the paste configuration accepts.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addAcceptableTypeIdentifiers(_ acceptableTypeIdentifiers: [String])
```

## Parameters 

`acceptableTypeIdentifiers`  

An array of uniform type identifier (UTI) strings.

## Discussion

List the acceptable UTIs in descending order of fidelity. The UTI that provides the richest data representation should be first in the list. For instance, if the data to paste is contact information, list the vCard UTI first, followed by the plain text UTI.

## See Also

### Adding acceptable type identifiers

func addTypeIdentifiers(forAccepting: any NSItemProviderReading.Type)

Expands the array of accepted UTIs for a paste configuration, based on those declared as supported by a specified class.

func addTypeIdentifiers&lt;T>(forAccepting: T.Type)

