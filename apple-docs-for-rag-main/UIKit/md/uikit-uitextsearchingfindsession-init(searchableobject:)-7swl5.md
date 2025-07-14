

- UIKit
- UITextSearchingFindSession
-  init(searchableObject:) 

Initializer

# init(searchableObject:)

Initializes an object to manage the search for the searchable object you specify.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(searchableObject: SearchableObject) where SearchableObject : UITextSearching
```

## Parameters 

`searchableObject`  

An object that conforms to the UITextSearching protocol that the session uses to search the text of your app and decorate the found results.

## See Also

### Creating a text searching find session

init(searchableObject: any __UITextSearching)

Initializes an object to manage the search for the searchable object you specify.

