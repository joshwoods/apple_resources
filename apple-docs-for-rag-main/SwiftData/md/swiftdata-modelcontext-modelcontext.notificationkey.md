

- SwiftData
- ModelContext
-  ModelContext.NotificationKey 

Enumeration

# ModelContext.NotificationKey

Describes the data in the user info dictionary of a notification sent by a model context.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
enum NotificationKey
```

## Topics

### Accessing notification keys

case deletedIdentifiers

A set of values identifying the context’s deleted models.

case insertedIdentifiers

A set of values identifying the context’s inserted models.

case invalidatedAllIdentifiers

A set of values identifying the context’s invalidated models.

case updatedIdentifiers

A set of values identifying the context’s updated models.

case queryGeneration

A token that indicates which generation of the model store SwiftData is using.

### Creating a notification key

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Registering for notifications

static let willSave: Notification.Name

A notification that posts when the context is about to process pending inserts, changes, and deletes.

static let didSave: Notification.Name

A notification that posts when the context finishes processing pending inserts, changes, and deletes.

