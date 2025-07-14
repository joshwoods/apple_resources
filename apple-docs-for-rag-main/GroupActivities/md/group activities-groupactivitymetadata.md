

- Group Activities
-  GroupActivityMetadata 

Structure

# GroupActivityMetadata

Text and image content that describes an activity to potential participants.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct GroupActivityMetadata
```

## Mentioned in 

Defining your app’s SharePlay activities

Adding spatial Persona support to an activity

## Overview

Use a `GroupActivityMetadata` structure to store user-facing information about a specific activity your app suggests. Metadata information includes the title of the activity, an image that corresponds to the activity, and a fallback URL for users who don’t have your app. For example, a movie-watching activity might include the poster of the specific movie a participant suggests. The system uses the provided metadata to generate invitations for other participants.

Create a `GroupActivityMetadata` structure in the metadata property of your custom GroupActivity subclass. Populate the new structure with the relevant data for your activity.

## Topics

### Creating group activity metadata

init()

Creates a new instance for storing descriptive information about an activity.

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Presenting the activity

var title: String?

The localized string to display as the title of your activity.

var subtitle: String?

The localized string that provides additional information about the activity.

var previewImage: CGImage?

The image to display for the current activity.

var fallbackURL: URL?

A URL that offers participants a way to identify or join the activity from a web browser.

### Indicating the activity’s type

var type: GroupActivityMetadata.ActivityType

The type of shared experience.

struct ActivityType

Constants that indicate the group activity’s type to the system.

### Assigning an app-specific scene

var sceneAssociationBehavior: SceneAssociationBehavior

Criteria the system uses to direct an activity to a specific scene of your app.

struct SceneAssociationBehavior

A type that tells the system which scene to associate with an incoming group activity.

### Specifying media-related behavior

var supportsContinuationOnTV: Bool

A Boolean value that indicates whether your app supports activity continuation on an Apple TV.

var preferredBroadcastOptions: BroadcastOptions

Preferences for how to present audio and video on the main communication channel.

struct BroadcastOptions

Options for how to broadcast media on the shared communications channel.

### Comparing metadata objects

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (GroupActivityMetadata, GroupActivityMetadata) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Encoding the metadata

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Structures

struct LifetimePolicy

An activity lifetime policy used by a Group Activity.

### Instance Properties

var experience: GroupActivityMetadata.Experience?Deprecated

var lifetimePolicy: GroupActivityMetadata.LifetimePolicy

Determines how an activity can be ended.

var localizedSubtitle: String?Deprecated

var localizedTitle: String?Deprecated

### Enumerations

enum ExperienceDeprecated

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Activity definition

Defining your app’s SharePlay activities

Configure your app’s SharePlay support and define the activities that people can perform from your app.

Supporting Coordinated Media Playback

Create synchronized media experiences that enable users to watch and listen across devices.

protocol GroupActivity

A type that can advertise your app’s activities to other participants.

enum GroupActivityActivationResult

The result of preparing to start a custom activity.

struct GroupActivityTransferRepresentation

A type that lets you start a group activity from a known context.

