

- Core Animation
- CAMediaTimingFillMode
-  forwards 

Type Property

# forwards

The receiver remains visible in its final state when the animation is completed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
static let forwards: CAMediaTimingFillMode
```

## See Also

### Constants

static let removed: CAMediaTimingFillMode

The receiver is removed from the presentation when the animation is completed.

static let backwards: CAMediaTimingFillMode

The receiver clamps values before zero to zero when the animation is completed.

static let both: CAMediaTimingFillMode

The receiver clamps values at both ends of the object’s time space

