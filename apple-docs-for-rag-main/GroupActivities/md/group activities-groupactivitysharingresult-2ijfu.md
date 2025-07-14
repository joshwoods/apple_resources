

- Group Activities
-  GroupActivitySharingResult 

Enumeration

# GroupActivitySharingResult

The result of a request to share a group activity in iOS.

GroupActivitiesUIKitiOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
enum GroupActivitySharingResult
```

## Topics

### Getting the result

case success

A result that indicates someone wants to share the activity with the group.

case cancelled

A result that indicates someone canceled the request.

### Comparing results

static func == (GroupActivitySharingResult, GroupActivitySharingResult) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Getting the hash value

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Instance Properties

var hashValue: Int

The hash value.

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

