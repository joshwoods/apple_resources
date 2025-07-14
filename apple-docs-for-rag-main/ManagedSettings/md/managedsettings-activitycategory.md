

- ManagedSettings
-  ActivityCategory 

Structure

# ActivityCategory

An activity’s category, such as Entertainment or Social.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct ActivityCategory
```

## Topics

### Creating a Category

init(token: ActivityCategoryToken)

Initializes the representation with the provided token.

### Accessing Category Identifiers

let localizedDisplayName: String?

A localized display name for the category.

let token: ActivityCategoryToken?

An opaque representation of a category of activities.

### Comparing Categories

static func == (ActivityCategory, ActivityCategory) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value that indicates whether two values aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Categories

typealias ActivityCategoryToken

A token that represents a category of app or website activity.

