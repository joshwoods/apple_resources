

- App Intents
-  ConfirmationActionName 

Structure

# ConfirmationActionName

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ConfirmationActionName
```

## Topics

### Type Properties

static var add: ConfirmationActionName

static var addData: ConfirmationActionName

static var book: ConfirmationActionName

static var buy: ConfirmationActionName

static var call: ConfirmationActionName

static var checkIn: ConfirmationActionName

static var `continue`: ConfirmationActionName

static var create: ConfirmationActionName

static var `do`: ConfirmationActionName

static var download: ConfirmationActionName

static var filter: ConfirmationActionName

static var find: ConfirmationActionName

static var get: ConfirmationActionName

static var go: ConfirmationActionName

static var log: ConfirmationActionName

static var open: ConfirmationActionName

static var order: ConfirmationActionName

static var pay: ConfirmationActionName

static var play: ConfirmationActionName

static var playSound: ConfirmationActionName

static var post: ConfirmationActionName

static var request: ConfirmationActionName

static var run: ConfirmationActionName

static var search: ConfirmationActionName

static var send: ConfirmationActionName

static var set: ConfirmationActionName

static var share: ConfirmationActionName

static var start: ConfirmationActionName

static var startNavigation: ConfirmationActionName

static var toggle: ConfirmationActionName

static var turnOff: ConfirmationActionName

static var turnOn: ConfirmationActionName

static var view: ConfirmationActionName

### Type Methods

static func custom(acceptLabel: LocalizedStringResource, acceptAlternatives: [LocalizedStringResource], denyLabel: LocalizedStringResource, denyAlternatives: [LocalizedStringResource], destructive: Bool) -> ConfirmationActionName

## Relationships

### Conforms To

- Sendable

## See Also

### Responding to the Action button

Responding to the Action button on Apple Watch Ultra

Use App Intents to register actions for your app.

protocol StartWorkoutIntent

An App Intent for starting a workout.

protocol PauseWorkoutIntent

An App Intent that lets someone pause your app’s current workout session.

protocol ResumeWorkoutIntent

An App Intent that lets someone resume your app’s paused workout session.

protocol StartDiveIntent

An App Intent that lets people start a dive session when they press the Action button on Apple Watch Ultra.

