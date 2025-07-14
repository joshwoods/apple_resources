

- App Intents
- EntityIdentifier
-  identifier 

Instance Property

# identifier

Value uniquely identifying the entity instance within its type

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let identifier: String
```

## See Also

### Getting the identifier details

let entityType: any AppEntity.Type

The type of `AppEntity` represented by this identifier

static let valueMaximumLength: Int

Maximum allowed length for the `identifier` value. This is a constraint imposed by the system and thus forces us to truncate the identifier if it exceeds the maximum length.

