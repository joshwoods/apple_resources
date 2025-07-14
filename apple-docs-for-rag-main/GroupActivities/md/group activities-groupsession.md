

- Group Activities
-  GroupSession 

Class

# GroupSession

A session for an in-progress activity that synchronizes content among participant devices.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final class GroupSession where ActivityType : GroupActivity
```

## Mentioned in 

Joining and managing a shared activity

Adding spatial Persona support to an activity

Synchronizing data during a SharePlay activity

## Overview

A `GroupSession` object contains details about the user’s currently selected activity, its status, and its participants. When a participant engages in an activity, the system binds a session to that activity for you. You use the session object to synchronize your app’s activity-related content, including your app’s UI.

You don’t create `GroupSession` objects directly. Instead, the system creates sessions and makes them available to your app asynchronously. Use the `AsyncSequence` type returned by the sessions() method of your activity to retrieve new sessions when they become available.

Before the system can create a session object, your app must create a `GroupActivity` object and activate it. For information about how to configure group activities, see GroupActivity.

### Start and Stop the Session

When you receive a new session object, it’s initially in the GroupSession.State.waiting state. As soon as your app is ready to begin the associated activity, call the session’s join() method. Joining a session validates the connection and starts the synchronization process between the current device and other participants’ devices. If your app successfully joins the session, the session transitions to the GroupSession.State.joined state.

When the user quits your app, or navigates away from the shared activity, call the session’s leave() method. Leaving a session gracefully transitions it to the GroupSession.State.invalidated(reason:) state, and informs the system that the user isn’t currently engaged in the activity.

## Topics

### Getting the current session

struct Sessions

An asynchronous sequence of sessions you use to manage a specific activity.

### Joining and leaving the session

func join()

Starts the shared activity on the current device.

func leave()

Leaves the current activity and stops receiving synchronized data.

func end()

Ends the activity for the entire group and stops the transfer of synchronized data.

### Accessing the shared activity

var activity: ActivityType

The current activity associated with the session.

### Getting the session details

var state: GroupSession&lt;ActivityType>.State

The current state of the session.

enum State

The possible states of a session.

let id: UUID

The unique identifier of the current session.

var description: String

A textual representation of this instance.

### Getting the participants

var localParticipant: Participant

The participant on the current device.

var activeParticipants: Set&lt;Participant>

The set of participants currently engaged in the activity.

### Getting the scene-association identifier

var sceneSessionIdentifier: String?

The persistent identifier of the session’s associated scene.

### Getting the participant’s attention

func requestForegroundPresentation()

Tells the system that your app needs to be in the foreground to continue an activity.

### Notifying participants of playback changes

func showNotice(GroupSessionEvent)

Posts an event to the system, which displays the information in the system UI.

struct GroupSessionEvent

A session-related event that appears in the system UI.

### Publishing changes

var objectWillChange: ObservableObjectPublisher

### Structures

struct Event

A session-related event to display in the system UI.

Deprecated

### Instance Properties

var $activeParticipants: Published&lt;Set&lt;Participant>>.Publisher

var $activity: Published&lt;ActivityType>.Publisher

var $state: Published&lt;GroupSession&lt;ActivityType>.State>.Publisher

let isLocallyInitiated: Bool

A Boolean value that is true if the current session was created by the local participant.

var systemCoordinator: SystemCoordinator?

The system coordinator associated with an active session.

### Instance Methods

func postEvent(GroupSession&lt;ActivityType>.Event)

Posts an event to the system, which displays the information in the system UI.

Deprecated

### Type Aliases

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

### Default Implementations

CustomStringConvertible Implementations

ObservableObject Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- ObservableObject

## See Also

### Session management

Joining and managing a shared activity

Configure the session when a SharePlay activity starts, and handle events that occur during the lifetime of the activity.

Drawing content in a group session

Invite your friends to draw on a shared canvas while on a FaceTime call.

protocol CustomMessageIdentifiable

A type that assigns a custom ID string to messages you send to other devices.

struct Participant

An active participant in a group session.

