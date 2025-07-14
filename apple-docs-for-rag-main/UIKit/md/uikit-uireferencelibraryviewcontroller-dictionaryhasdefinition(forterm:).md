

- UIKit
- UIReferenceLibraryViewController
-  dictionaryHasDefinition(forTerm:) 

Type Method

# dictionaryHasDefinition(forTerm:)

Returns whether a definition is available for the given term.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func dictionaryHasDefinition(forTerm term: String) -> Bool
```

## Parameters 

`term`  

The term to be defined.

## Return Value

true if a definition for `term` is available; otherwise, false.

## See Also

### Creating a reference-library view controller

init(term: String)

Initializes a newly created reference-library view controller to display the definition of the given term.

init(coder: NSCoder)

Creates a reference-library view controller from data in an unarchiver.

