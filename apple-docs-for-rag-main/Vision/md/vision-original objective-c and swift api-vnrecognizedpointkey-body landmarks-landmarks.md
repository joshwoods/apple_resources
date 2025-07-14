

- Vision
- Original Objective-C and Swift API
- VNRecognizedPointKey
-  Body Landmarks 

API Collection

# Body Landmarks

The body landmarks that Vision detects.

## Overview

The illustration below shows the nineteen body points that you can detect with VNDetectHumanBodyPoseRequest.

## Topics

### Head

static let bodyLandmarkKeyLeftEye: VNRecognizedPointKey

The left eye.

Deprecated

static let bodyLandmarkKeyRightEye: VNRecognizedPointKey

The right eye.

Deprecated

static let bodyLandmarkKeyLeftEar: VNRecognizedPointKey

The left ear.

Deprecated

static let bodyLandmarkKeyRightEar: VNRecognizedPointKey

The right ear.

Deprecated

static let bodyLandmarkKeyNose: VNRecognizedPointKey

The nose.

Deprecated

static let bodyLandmarkRegionKeyFace: VNRecognizedPointGroupKey

A group key identifying the face, which includes the eyes, ears, and nose.

Deprecated

### Torso

static let bodyLandmarkKeyNeck: VNRecognizedPointKey

The center point of the neck.

Deprecated

static let bodyLandmarkKeyLeftShoulder: VNRecognizedPointKey

The left shoulder.

Deprecated

static let bodyLandmarkKeyRightShoulder: VNRecognizedPointKey

The right shoulder.

Deprecated

static let bodyLandmarkKeyLeftHip: VNRecognizedPointKey

The left hip.

Deprecated

static let bodyLandmarkKeyRightHip: VNRecognizedPointKey

The right hip.

Deprecated

static let bodyLandmarkKeyRoot: VNRecognizedPointKey

The center point of the waist.

Deprecated

static let bodyLandmarkRegionKeyTorso: VNRecognizedPointGroupKey

A group key identifying the torso, which includes the neck, shoulders, hips, and root.

Deprecated

### Arms

static let bodyLandmarkKeyRightWrist: VNRecognizedPointKey

The right wrist.

Deprecated

static let bodyLandmarkKeyRightElbow: VNRecognizedPointKey

The right elbow.

Deprecated

static let bodyLandmarkRegionKeyRightArm: VNRecognizedPointGroupKey

A group key identifying the landmarks of the right arm.

Deprecated

static let bodyLandmarkKeyLeftWrist: VNRecognizedPointKey

The left wrist.

Deprecated

static let bodyLandmarkKeyLeftElbow: VNRecognizedPointKey

The left elbow.

Deprecated

static let bodyLandmarkRegionKeyLeftArm: VNRecognizedPointGroupKey

A group key identifying the landmarks of the left arm.

Deprecated

### Legs

static let bodyLandmarkKeyRightKnee: VNRecognizedPointKey

The right knee.

Deprecated

static let bodyLandmarkKeyRightAnkle: VNRecognizedPointKey

The right ankle.

Deprecated

static let bodyLandmarkRegionKeyRightLeg: VNRecognizedPointGroupKey

A group key identifying the landmarks of the right leg.

Deprecated

static let bodyLandmarkKeyLeftKnee: VNRecognizedPointKey

The left knee.

Deprecated

static let bodyLandmarkKeyLeftAnkle: VNRecognizedPointKey

The left ankle.

Deprecated

static let bodyLandmarkRegionKeyLeftLeg: VNRecognizedPointGroupKey

A group key identifying the landmarks of the left leg.

Deprecated

### All Landmarks

static let all: VNRecognizedPointGroupKey

A group key identifying all landmarks.

## See Also

### Landmarks

Hand Landmarks

The hand landmarks that Vision detects.

