

- Core Animation
- CAMediaTimingFunction
-  Predefined Timing Functions 

API Collection

# Predefined Timing Functions

Constants that specify system-provided timing functions, used by init(name:).

## Topics

### Constants

static let linear: CAMediaTimingFunctionName

Linear pacing, which causes an animation to occur evenly over its duration.

static let easeIn: CAMediaTimingFunctionName

Ease-in pacing, which causes an animation to begin slowly and then speed up as it progresses.

static let easeOut: CAMediaTimingFunctionName

Ease-out pacing, which causes an animation to begin quickly and then slow as it progresses.

static let easeInEaseOut: CAMediaTimingFunctionName

Ease-in-ease-out pacing, which causes an animation to begin slowly, accelerate through the middle of its duration, and then slow again before completing.

static let `default`: CAMediaTimingFunctionName

The system default timing function. Use this function to ensure that the timing of your animations matches that of most system animations.

