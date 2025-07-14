

- UIKit
- UIReferenceLibraryViewController
-  init(term:) 

Initializer

# init(term:)

Initializes a newly created reference-library view controller to display the definition of the given term.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(term: String)
```

## Parameters 

`term`  

The term to define.

## Return Value

The newly initialized reference library view controller.

## Discussion

If a definition for the term is not available, a localized message is displayed instead. Use the dictionaryHasDefinition(forTerm:) class method to determine whether a definition is available before creating instances of this class.

## See Also

### Creating a reference-library view controller

class func dictionaryHasDefinition(forTerm: String) -> Bool

Returns whether a definition is available for the given term.

init(coder: NSCoder)

Creates a reference-library view controller from data in an unarchiver.

