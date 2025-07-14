

- ContactProvider
- ContactItem
-  ContactItem.Identifier 

Structure

# ContactItem.Identifier

The app’s identifier for an item in the contact database.

iOS 18.0+iPadOS 18.0+

``` source
struct Identifier
```

## Topics

### Creating a contact item identifier

init(String)

Creates an identifier with the given value.

### Inspecting identifier properties

let value: String

The value of the identifier.

### Accessing the root container

static let rootContainer: ContactItem.Identifier

The top-level container, containing the user’s contacts.

### Operators

static func == (ContactItem.Identifier, ContactItem.Identifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

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

- Equatable
- Hashable

