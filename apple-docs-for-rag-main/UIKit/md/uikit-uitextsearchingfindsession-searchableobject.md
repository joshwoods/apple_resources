

- UIKit
- UITextSearchingFindSession
-  searchableObject 

Instance Property

# searchableObject

The object to search, responsible for performing the search operation and decorating the results.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
weak var searchableObject: (any __UITextSearching)? { get }
```

## Discussion

Use the methods this object implements from the UITextSearching protocol to search text in your app and decorate the found results.

