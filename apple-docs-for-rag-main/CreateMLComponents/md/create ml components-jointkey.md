

- Create ML Components
-  JointKey 

Structure

# JointKey

A key that uniquely identifies a joint.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct JointKey
```

## Topics

### Creating a joint key

init(rawValue: String)

Creates a new instance with the specified raw value.

### Getting elbow properties

static let leftElbow: JointKey

A key associated with left elbow joint in a body pose.

static let rightElbow: JointKey

A key associated with right elbow joint in a body pose.

### Getting head properties

static let leftEye: JointKey

A key associated with left eye joint in a body pose.

static let rightEye: JointKey

A key associated with right eye joint in a body pose.

static let leftEar: JointKey

A key associated with left ear joint in a body pose.

static let rightEar: JointKey

A key associated with right ear joint in a body pose.

static let nose: JointKey

A key associated with nose joint in a body pose.

### Getting index finger properties

static let indexDIP: JointKey

A key associated with index finger’s distal interphalangeal (DIP) joint in a hand pose.

static let indexMCP: JointKey

A key associated with index finger’s metacarpophalangeal (MCP) joint in a hand pose.

static let indexPIP: JointKey

A key associated with index finger’s proximal interphalangeal (PIP) joint in a hand pose.

static let indexTip: JointKey

A key associated with index finger tip joint in a hand pose.

### Getting little finger properties

static let littleDIP: JointKey

A key associated with ring finger’s distal interphalangeal (DIP) joint in a hand pose.

static let littleMCP: JointKey

A key associated with ring finger’s metacarpophalangeal (MCP) joint in a hand pose.

static let littlePIP: JointKey

A key associated with ring finger’s proximal interphalangeal (PIP) joint in a hand pose.

static let littleTip: JointKey

A key associated with ring finger tip joint in a hand pose.

### Getting middle finger properties

static let middleDIP: JointKey

A key associated with middle finger’s distal interphalangeal (DIP) joint in a hand pose.

static let middleMCP: JointKey

A key associated with middle finger’s metacarpophalangeal (MCP) joint in a hand pose.

static let middlePIP: JointKey

A key associated with middle finger’s proximal interphalangeal (PIP) joint in a hand pose.

static let middleTip: JointKey

A key associated with middle finger tip joint in a hand pose.

### Getting ring finger properties

static let ringDIP: JointKey

A key associated with ring finger’s distal interphalangeal (DIP) joint in a hand pose.

static let ringMCP: JointKey

A key associated with ring finger’s metacarpophalangeal (MCP) joint in a hand pose.

static let ringPIP: JointKey

A key associated with ring finger’s proximal interphalangeal (PIP) joint in a hand pose.

static let ringTip: JointKey

A key associated with ring finger tip joint in a hand pose.

### Getting thumb properties

static let thumbCMC: JointKey

A key associated with thumb carpometacarpal (CMC) joint in a hand pose.

static let thumbIP: JointKey

A key associated with thumb interphalangeal (IP) joint in a hand pose.

static let thumbMP: JointKey

A key associated with thumb metacarpophalangeal (MP) joint in a hand pose.

static let thumbTip: JointKey

A key associated with thumb tip joint in a hand pose.

### Getting wrist properties

static let leftWrist: JointKey

A key associated with left wrist joint in a body pose.

static let rightWrist: JointKey

A key associated with right wrist joint in a body pose.

static let wrist: JointKey

A key associated with hand wrist joint in a hand pose.

### Getting neck and shoulder properties

static let neck: JointKey

A key associated with neck joint in a body pose.

static let leftShoulder: JointKey

A key associated with left shoulder joint in a body pose.

static let rightShoulder: JointKey

A key associated with right shoulder joint in a body pose.

### Getting hip, knee, and ankle properties

static let leftHip: JointKey

A key associated with left hip joint in a body pose.

static let leftKnee: JointKey

A key associated with left knee joint in a body pose.

static let rightHip: JointKey

A key associated with right hip joint in a body pose.

static let rightKnee: JointKey

A key associated with right knee joint in a body pose.

static let leftAnkle: JointKey

A key associated with left ankle joint in a body pose.

static let rightAnkle: JointKey

A key associated with right ankle joint in a body pose.

### Getting root and raw Properties

static let root: JointKey

A key associated with root joint in a body pose.

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Pose components

Counting human body action repetitions in a live video feed

Use Create ML Components to analyze a series of video frames and count a person’s repetitive or periodic body movements.

struct Pose

A pose that contains joint keypoints from a person, a hand, or a combination.

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

