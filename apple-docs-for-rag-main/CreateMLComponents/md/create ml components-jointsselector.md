

- Create ML Components
-  JointsSelector 

Structure

# JointsSelector

Joints selector from a pose.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct JointsSelector
```

## Topics

### Creating a selector

init(ignoredJoints: [JointKey])

Creates a joint selector transformer using a list of joint keys to be ignored.

init(selectedJoints: [JointKey])

Creates a joint selector transformer using a list of joint keys to be selected.

### Getting the properties

var ignoredJoints: [JointKey]?

A list of joint keys to be ignored.

var selectedJoints: [JointKey]?

A list of joint keys to be selected.

### Performing the selector

func applied(to: Pose, eventHandler: EventHandler?) -> Pose

Select joints to be included in the pose. Ignored joints will be reset to zero in all fields.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Sendable
- Transformer

## See Also

### Pose components

Counting human body action repetitions in a live video feed

Use Create ML Components to analyze a series of video frames and count a person’s repetitive or periodic body movements.

struct Pose

A pose that contains joint keypoints from a person, a hand, or a combination.

struct JointKey

A key that uniquely identifies a joint.

struct JointPoint

A joint in a pose that contains a location and scoring information.

struct PoseSelector

A transformer that selects one pose from an array of poses.

enum PoseSelectionStrategy

Pose selection strategy.

struct HumanBodyPoseExtractor

The human body pose image feature extractor.

struct HumanHandPoseExtractor

The human hand pose image feature extractor.

struct HumanBodyActionCounter

A human body action repetition counting transformer that takes window of human body poses and produces cumulative human body action repetition counts.

struct HumanBodyActionPeriodPredictor

A human body action period predictor transformer that takes window of poses and produces a window of predictions.

