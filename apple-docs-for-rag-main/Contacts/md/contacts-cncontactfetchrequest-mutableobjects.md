

- Contacts
- CNContactFetchRequest
-  mutableObjects 

Instance Property

# mutableObjects

A Boolean value that indicates whether to return mutable contacts.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
var mutableObjects: Bool { get set }
```

## Discussion

When the value of this property is true, the fetch returns CNMutableContact objects; otherwise it returns CNContact objects. The default value of this property is false.

## See Also

### Configuring the Fetch Options

var unifyResults: Bool

A Boolean value that indicates whether to return linked contacts as unified contacts.

var sortOrder: CNContactSortOrder

The sort order for contacts.

enum CNContactSortOrder

Indicates the sorting order for contacts.

