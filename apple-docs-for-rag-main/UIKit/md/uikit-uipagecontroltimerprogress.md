

- UIKit
-  UIPageControlTimerProgress 

Class

# UIPageControlTimerProgress

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
class UIPageControlTimerProgress
```

## Topics

### Initializers

init(preferredDuration: TimeInterval)

### Instance Properties

var delegate: (any UIPageControlTimerProgressDelegate)?

var isRunning: Bool

var preferredDuration: TimeInterval

var resetsToInitialPageAfterEnd: Bool

### Instance Methods

func duration(forPage: Int) -> TimeInterval

func pauseTimer()

func resumeTimer()

func setDuration(TimeInterval, forPage: Int)

## Relationships

### Inherits From

- UIPageControlProgress

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring page progress

var progress: UIPageControlProgress?

class UIPageControlProgress

protocol UIPageControlProgressDelegate

protocol UIPageControlTimerProgressDelegate

