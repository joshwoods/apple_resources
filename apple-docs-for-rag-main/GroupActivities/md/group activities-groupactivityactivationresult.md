

- Group Activities
-  GroupActivityActivationResult 

Enumeration

# GroupActivityActivationResult

The result of preparing to start a custom activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum GroupActivityActivationResult
```

## Overview

When you call prepareForActivation(), the system determines whether you share the activity with other participants in a FaceTime call, or perform it locally. After making the determination, it passes a `GroupActivityActivationResult` value to the method’s completion handler. Use that value to start the activity in the selected setting.

## Topics

### Getting the activation results

case activationPreferred

A result that indicates the user wants to share the activity with the group.

case activationDisabled

A result that indicates the user disabled the automatic sharing of activities, or prefers to perform the activity locally.

case cancelled

A result that indicates the user canceled the activation request.

### Comparing reliability options

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (GroupActivityActivationResult, GroupActivityActivationResult) -> Bool

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

- Copyable
- Equatable
- Hashable
- Sendable

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

struct GroupActivityTransferRepresentation

A type that lets you start a group activity from a known context.

