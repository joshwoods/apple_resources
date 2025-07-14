

- Core Animation
- CAMediaTiming
-  Fill Modes 

API Collection

# Fill Modes

These constants determine how the timed object behaves once its active duration has completed. They are used with the fillMode property.

## Topics

### Constants

static let removed: CAMediaTimingFillMode

The receiver is removed from the presentation when the animation is completed.

static let forwards: CAMediaTimingFillMode

The receiver remains visible in its final state when the animation is completed.

static let backwards: CAMediaTimingFillMode

The receiver clamps values before zero to zero when the animation is completed.

static let both: CAMediaTimingFillMode

The receiver clamps values at both ends of the object’s time space

