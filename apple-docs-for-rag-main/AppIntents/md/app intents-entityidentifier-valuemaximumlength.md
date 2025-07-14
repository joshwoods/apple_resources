

- App Intents
- EntityIdentifier
-  valueMaximumLength 

Type Property

# valueMaximumLength

Maximum allowed length for the `identifier` value. This is a constraint imposed by the system and thus forces us to truncate the identifier if it exceeds the maximum length.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let valueMaximumLength: Int
```

## See Also

### Getting the identifier details

let identifier: String

Value uniquely identifying the entity instance within its type

let entityType: any AppEntity.Type

The type of `AppEntity` represented by this identifier

