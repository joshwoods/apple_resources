

- Create ML Components
-  JointPoint 

Structure

# JointPoint

A joint in a pose that contains a location and scoring information.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct JointPoint
```

## Topics

### Creating a joint point

init(JointKey, location: CGPoint, confidence: Float)

Creates a joint point with its key, location and confidence.

### Getting the detection confidence

var confidence: Float

A detection confidence of the joint

### Getting the key name

let key: JointKey

The key name for the joint

### Getting the joint location

var location: CGPoint

The location of the joint point

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Pose components

Counting human body action repetitions in a live video feed

Use Create ML Components to analyze a series of video frames and count a person’s repetitive or periodic body movements.

struct Pose

A pose that contains joint keypoints from a person, a hand, or a combination.

struct JointKey

A key that uniquely identifies a joint.

struct PoseSelector

A transformer that selects one pose from an array of poses.

enum PoseSelectionStrategy

Pose selection strategy.

struct JointsSelector

Joints selector from a pose.

struct HumanBodyPoseExtractor

The human body pose image feature extractor.

struct HumanHandPoseExtractor

The human hand pose image feature extractor.

struct HumanBodyActionCounter

A human body action repetition counting transformer that takes window of human body poses and produces cumulative human body action repetition counts.

struct HumanBodyActionPeriodPredictor

A human body action period predictor transformer that takes window of poses and produces a window of predictions.

