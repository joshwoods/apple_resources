

- Group Activities
-  GroupActivityTransferRepresentation 

Structure

# GroupActivityTransferRepresentation

A type that lets you start a group activity from a known context.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct GroupActivityTransferRepresentation where Item : Transferable
```

## Mentioned in 

Defining your app’s SharePlay activities

Presenting SharePlay activities from your app’s UI

## Topics

### Initializers

init&lt;ActivityType>(exporting: (Item) async throws -> ActivityType)

Creates a type that exports a group activity for the specified item.

### Instance Properties

var body: some TransferRepresentation

A builder expression that describes the process of importing and exporting an item.

### Type Aliases

typealias Body

The transfer representation for the item.

### Default Implementations

TransferRepresentation Implementations

## Relationships

### Conforms To

- Sendable
- TransferRepresentation

## See Also

### Activity definition

Defining your app’s SharePlay activities

Configure your app’s SharePlay support and define the activities that people can perform from your app.

Supporting Coordinated Media Playback

Create synchronized media experiences that enable users to watch and listen across devices.

protocol GroupActivity

A type that can advertise your app’s activities to other participants.

struct GroupActivityMetadata

Text and image content that describes an activity to potential participants.

enum GroupActivityActivationResult

The result of preparing to start a custom activity.

