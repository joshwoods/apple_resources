

- Group Activities
- GroupActivityMetadata
-  GroupActivityMetadata.ActivityType 

Structure

# GroupActivityMetadata.ActivityType

Constants that indicate the group activity’s type to the system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct ActivityType
```

## Topics

### Getting the Activity Types

static let generic: GroupActivityMetadata.ActivityType

A generic activity.

static let listenTogether: GroupActivityMetadata.ActivityType

A shared listening activity, such as listening to music together.

static let watchTogether: GroupActivityMetadata.ActivityType

A shared watching activity, such as watching an episode of a television show together.

### Comparing Activity Types

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (GroupActivityMetadata.ActivityType, GroupActivityMetadata.ActivityType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let createTogether: GroupActivityMetadata.ActivityType

A shared creation activity, such as drawing on an art canvas together.

static let exploreTogether: GroupActivityMetadata.ActivityType

A shared exploration activity, such as planning a trip together or browsing a web feed together.

static let learnTogether: GroupActivityMetadata.ActivityType

A shared learning activity, such as studying a topic together.

static let readTogether: GroupActivityMetadata.ActivityType

A shared reading activity, such as reading a book together.

static let shopTogether: GroupActivityMetadata.ActivityType

A shared shopping activity, such as browsing for products online together.

static let workoutTogether: GroupActivityMetadata.ActivityType

A shared workout activity, such as participating in a fitness class together.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Indicating the activity’s type

var type: GroupActivityMetadata.ActivityType

The type of shared experience.

