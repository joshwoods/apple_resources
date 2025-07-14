

- Cinematic
- CNScript
-  CNScript.Frame 

Structure

# CNScript.Frame

An object that represents what to focus on, and where to focus, in a given movie frame.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
struct Frame
```

## Topics

### Instance Properties

var allDetections: [CNDetection]

All detections for the Cinematic movie.

var focusDetection: CNDetection

What to focus on in a given frame of the movie.

var focusDisparity: Float

Where to focus in a given frame of the movie.

var time: CMTime

The time of the focus transition.

### Instance Methods

func bestDetection(for: CNDetectionGroupID) -> CNDetection?

The best detection to focus on in a frame among those within the given detection group.

func detection(for: CNDetectionID) -> CNDetection?

The detection in the frame with the given detection ID, if any.

## Relationships

### Conforms To

- Sendable

