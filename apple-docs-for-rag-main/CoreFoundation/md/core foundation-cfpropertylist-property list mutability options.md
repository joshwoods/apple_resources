

- Core Foundation
- CFPropertyList
-  Property List Mutability Options 

API Collection

# Property List Mutability Options

Option flags that determine the degree of mutability of newly created property lists.

## Topics

### Constants

static var mutableContainers: CFPropertyListMutabilityOptions

Specifies that the property list should have mutable containers but immutable leaves.

static var mutableContainersAndLeaves: CFPropertyListMutabilityOptions

Specifies that the property list should have mutable containers and mutable leaves.

## See Also

### Constants

enum CFPropertyListFormat

Specifies the format of a property list.

Reading and Writing Error Codes

Error codes for property list reading and writing functions such as CFPropertyListCreateWithData(_:_:_:_:_:).

