

- AVKit
-  AVVideoFrameAnalysisType 

Structure

# AVVideoFrameAnalysisType

Constants that define the types of analysis a player view controller may perform on a paused video frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct AVVideoFrameAnalysisType
```

## Topics

### Analysis types

static var `default`: AVVideoFrameAnalysisType

The default types of analysis to perform.

static var text: AVVideoFrameAnalysisType

A type that finds text in a paused video frame.

static var subject: AVVideoFrameAnalysisType

A type that finds a subject that a user can copy out of frame.

static var visualSearch: AVVideoFrameAnalysisType

A type that identifies objects, landmarks, art, and so on.

static var machineReadableCode: AVVideoFrameAnalysisType

A type that recognizes machine-readable codes, such as QR codes.

### Initializers

init(rawValue: UInt)

Creates a type from a string value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring Frame Analysis

var allowsVideoFrameAnalysis: Bool

A Boolean value that indicates whether to perform video frame analysis.

var videoFrameAnalysisTypes: AVVideoFrameAnalysisType

