

- Group Activities
-  GroupActivitySharingResult 

Enumeration

# GroupActivitySharingResult

The result of a request to share a group activity in macOS.

GroupActivitiesAppKitmacOS 13.0+

``` source
enum GroupActivitySharingResult
```

## Topics

### Operators

static func == (GroupActivitySharingResult, GroupActivitySharingResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case cancelled

A result that indicates the user canceled the request.

case success

A result that indicates the user wants to share the activity with the group.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Getting the result

var result: GroupActivitySharingResult

The result of a request to share a group activity.

