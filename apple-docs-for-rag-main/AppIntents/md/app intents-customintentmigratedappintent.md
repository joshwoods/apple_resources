

- App Intents
-  CustomIntentMigratedAppIntent 

Protocol

# CustomIntentMigratedAppIntent

An interface for replacing a custom SiriKit intent that allows existing shortcuts and donations to continue working.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CustomIntentMigratedAppIntent : AppIntent
```

## Topics

### Specifying the migrated intent’s class name

static var intentClassName: String

The name of the SiriKit Intent class that this app intent replaces.

**Required**

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable

