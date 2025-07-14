

- Contacts
- CNContactFetchRequest
-  unifyResults 

Instance Property

# unifyResults

A Boolean value that indicates whether to return linked contacts as unified contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var unifyResults: Bool { get set }
```

## Discussion

A unified contact is an aggregation of properties from a set of linked individual contacts. When the value of this property is true, the fetch returns unified contacts; otherwise, it returns individual contacts. The default value of this property is true.

## See Also

### Configuring the Fetch Options

var mutableObjects: Bool

A Boolean value that indicates whether to return mutable contacts.

var sortOrder: CNContactSortOrder

The sort order for contacts.

enum CNContactSortOrder

Indicates the sorting order for contacts.

