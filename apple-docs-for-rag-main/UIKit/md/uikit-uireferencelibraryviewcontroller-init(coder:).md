

- UIKit
- UIReferenceLibraryViewController
-  init(coder:) 

Initializer

# init(coder:)

Creates a reference-library view controller from data in an unarchiver.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(coder: NSCoder)
```

## See Also

### Creating a reference-library view controller

class func dictionaryHasDefinition(forTerm: String) -> Bool

Returns whether a definition is available for the given term.

init(term: String)

Initializes a newly created reference-library view controller to display the definition of the given term.

