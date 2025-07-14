

- Create ML
-  MLProgress 

Structure

# MLProgress

A convenience type that exposes information about the progress of a training session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
struct MLProgress
```

## Overview

Create ML uses this type to exposes specific values within a *Progress* instance as properties.

## Topics

### Creating a training progress update

init(phase: MLPhase)

Creates a training session progress instance from a training phase.

init?(progress: Progress)

Creates a training session progress instance from a foundation progress object.

### Inspecting a session’s progress

var elapsedTime: TimeInterval

The time, in seconds, since the training session started.

var phase: MLPhase

The current phase of the training session.

var itemCount: Int

The current number of files processed during a feature extraction phase, or the completed iterations during a training phase.

var totalItemCount: Int?

The total number of files during a feature extraction phase, or total iterations during a training phase.

var metrics: [MLProgress.Metric : Any]

Measurements of the model’s performance during the training or evaluation phases of a training session.

enum Metric

Metrics you use to evaluate a model’s performance during a training session.

### Accessing general information

static let elapsedTimeKey: ProgressUserInfoKey

The key that accesses the elapsed time value.

static let phaseKey: ProgressUserInfoKey

The key that accesses the current phase value.

static let itemCountKey: ProgressUserInfoKey

The key that accesses the current item count value.

static let totalItemCountKey: ProgressUserInfoKey

The key that accesses the total item count value.

### Accessing assessment metrics

static let accuracyKey: ProgressUserInfoKey

The key that accesses the training accuracy value.

static let lossKey: ProgressUserInfoKey

The key that accesses the training loss value.

static let validationAccuracyKey: ProgressUserInfoKey

The key that accesses the validation accuracy value.

static let validationLossKey: ProgressUserInfoKey

The key that accesses the validation loss value.

### Accessing style transfer metrics

static let contentLossKey: ProgressUserInfoKey

The key that accesses the content image loss value.

static let styleLossKey: ProgressUserInfoKey

The key that accesses the style image loss value.

static let stylizedImageKey: ProgressUserInfoKey

The key that accesses the stylized image value.

### Accessing error information

static let maximumErrorKey: ProgressUserInfoKey

They key that accesses the maximum error value.

static let rootMeanSquaredErrorKey: ProgressUserInfoKey

They key that accesses the root-mean-squared error value.

static let validationMaximumErrorKey: ProgressUserInfoKey

They key that accesses the validation maximum error value.

static let validationRootMeanSquaredErrorKey: ProgressUserInfoKey

They key that accesses the validation root-mean-squared error value.

### Encoding and decoding a session’s progress

func encode(to: any Encoder) throws

Encodes the progress value into the given encoder.

init(from: any Decoder) throws

Creates a progress instance by decoding from the given decoder.

## Relationships

### Conforms To

- Decodable
- Encodable

## See Also

### Inspecting a job

let startDate: Date

The date and time when the training session began.

let progress: Progress

The training session’s current progress.

