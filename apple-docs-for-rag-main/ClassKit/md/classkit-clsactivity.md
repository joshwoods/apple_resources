

- ClassKit
-  CLSActivity 

Class

# CLSActivity

A representation of user interaction with a context.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
class CLSActivity
```

## Mentioned in 

Recording student progress

## Overview

An activity represents a student’s attempt to complete the task corresponding to a CLSContext instance. For example, if a context represents a quiz, the associated activity represents the student’s attempt to take the quiz. As such, an activity is always associated with a context. In fact, you never initialize an activity in isolation or store a reference to it. Rather, you ask a context to create the activity and retrieve it from the context.

### Starting and Stopping Activities

You start the activity with a call to the start() method when the user begins the task, and stop it with a call to the stop() method when the user finishes. You can also use the stop() method to stop it temporarily if the user pauses the task, in which case you can start it again later with another call to start() when the user resumes. The activity keeps track of the total time spent in the running state, which you can read via the duration property.

Whether you implement activity pausing depends on how the parts of your app work. For example, you might pause a game activity when the user presses the pause button to reflect that the user has stepped away from the activity, but is likely to return soon to complete the task. On the other hand, you might not provide a way to pause a quiz activity because you require that it be completed without interruption, once started. If you do pause, you can start and stop an activity as many times as you want, but when you create a new activity (representing a new attempt at a task), you can no longer access the older activity from your app.

### Recording Progress

You can also assign progress to an activity. How you define progress depends on the task being measured. For example, progress through a quiz can be recorded as the fraction of questions answered, while progress through a game level might be calculated as the fraction of obstacles overcome.

To record additional metrics, you attach CLSActivityItem instances to an activity. For example, you can add both a score and a count of hints used to a quiz activity. If one of these items should be featured prominently, you can make it the primaryActivityItem.

## Topics

### Starting and stopping an activity

func start()

Tells an activity to start recording duration and progress for a task.

func stop()

Tells an activity to stop or pause recording duration and progress for a task.

var isStarted: Bool

A Boolean that indicates whether an activity is running.

var duration: TimeInterval

The cumulative time in seconds that an activity has been active.

### Measuring progress

var progress: Double

A measure of progress through the task, given as a fraction in the range \[0, 1\].

func addProgressRange(fromStart: Double, toEnd: Double)

Adds a progress range to a given activity.

### Managing activity items

func addAdditionalActivityItem(CLSActivityItem)

Adds an activity item to an activity.

var primaryActivityItem: CLSActivityItem?

Adds an activity item to an activity and sets it as the primary activity item.

var additionalActivityItems: [CLSActivityItem]

The list of activity items associated with an activity.

func removeAllActivityItems()

Deletes all activity items associated with the current activity.

## Relationships

### Inherits From

- CLSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Activities

Recording student progress

Create an activity to record student progress through an assignment.

