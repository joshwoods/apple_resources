

- Create ML Components
-  Pose 

Structure

# Pose

A pose that contains joint keypoints from a person, a hand, or a combination.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Pose
```

## Topics

### Creating a pose

init(VNRecognizedPointsObservation) throws

Creates a pose from a body or hand pose observation.

init(from: [JointKey : JointPoint])

Creates a pose from a dictionary of joint keypoints.

### Getting the key points

var keypoints: [JointKey : JointPoint]

A dictionary of all keypoints in the pose

### Computing the bounding box

func boundingBoxArea(confidenceThreshold: Float) -> Float

Computes the bounding box area of the pose.

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

### Pose components

Counting human body action repetitions in a live video feed

Use Create ML Components to analyze a series of video frames and count a person’s repetitive or periodic body movements.

struct JointKey

A key that uniquely identifies a joint.

struct JointPoint

A joint in a pose that contains a location and scoring information.

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

