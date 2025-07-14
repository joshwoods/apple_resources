

- Create ML Components
-  HumanBodyPoseExtractor 

Structure

# HumanBodyPoseExtractor

The human body pose image feature extractor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct HumanBodyPoseExtractor
```

## Topics

### Creating the extractor

init()

Creates a human body pose extractor transformer

### Extracting the body pose

func applied(to: CIImage, eventHandler: EventHandler?) async throws -> [Pose]

Extracts human body poses from a pixel buffer.

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

struct JointsSelector

Joints selector from a pose.

struct HumanHandPoseExtractor

The human hand pose image feature extractor.

struct HumanBodyActionCounter

A human body action repetition counting transformer that takes window of human body poses and produces cumulative human body action repetition counts.

struct HumanBodyActionPeriodPredictor

A human body action period predictor transformer that takes window of poses and produces a window of predictions.

