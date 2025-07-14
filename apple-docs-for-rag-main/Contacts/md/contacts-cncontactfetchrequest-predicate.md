

- Contacts
- CNContactFetchRequest
-  predicate 

Instance Property

# predicate

The predicate to match contacts against.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var predicate: NSPredicate? { get set }
```

## Discussion

Set the value of this property to `nil` to match all contacts or use the search predicates in CNContact. Compound predicates are not supported.

