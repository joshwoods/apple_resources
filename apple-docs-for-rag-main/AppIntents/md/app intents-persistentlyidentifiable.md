

- App Intents
-  PersistentlyIdentifiable 

Protocol

# PersistentlyIdentifiable

Defines a string that uniquely identifies a type. This is useful for maintaining the identity of a type, even when its type name is changed.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PersistentlyIdentifiable
```

## Topics

### Type Properties

static var persistentIdentifier: String

A string that uniquely identifies this type.

**Required** Default implementations provided.

## Relationships

### Inherited By

- AppEntity
- AppEnum
- AppIntent
- AppValue
- AssistantEntity
- AssistantEnum
- AssistantIntent
- AssistantSchemaEntity
- AssistantSchemaEnum
- AssistantSchemaIntent
- AudioPlaybackIntent
- AudioRecordingIntent
- AudioStartingIntent
- CameraCaptureIntent
- ControlConfigurationIntent
- CustomIntentMigratedAppIntent
- DeleteIntent
- DeprecatedAppIntent
- EntityPropertyQuery
- EntityQuery
- EntityStringQuery
- EnumerableEntityQuery
- FileEntity
- ForegroundContinuableIntent
- IndexedEntity
- LiveActivityIntent
- LiveActivityStartingIntent
- OpenIntent
- PauseWorkoutIntent
- PlayVideoIntent
- PredictableIntent
- ProgressReportingIntent
- PushToTalkTransmissionIntent
- ResumeWorkoutIntent
- SetFocusFilterIntent
- SetValueIntent
- ShowInAppSearchResultsIntent
- StartDiveIntent
- StartWorkoutIntent
- SystemIntent
- TransientAppEntity
- URLRepresentableEntity
- URLRepresentableEnum
- URLRepresentableIntent
- UniqueAppEntity
- UniqueAppEntityQuery
- WidgetConfigurationIntent

### Conforming Types

- OpenURLIntent
- StringSearchScope
- UniqueAppEntityProvider
- VideoCategory

## See Also

### Entity identity

struct EntityIdentifier

A type that uniquely identifies a specific instance of an app entity.

protocol EntityIdentifierConvertible

An interface for converting between an entity’s identifier and its string representation.

