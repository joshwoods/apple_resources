

- UIKit
-  UIPageControlProgressDelegate 

Protocol

# UIPageControlProgressDelegate

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
protocol UIPageControlProgressDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func pageControlProgress(UIPageControlProgress, initialProgressForPage: Int) -> Float

func pageControlProgressVisibilityDidChange(UIPageControlProgress)

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UIPageControlTimerProgressDelegate

## See Also

### Configuring page progress

var progress: UIPageControlProgress?

class UIPageControlProgress

class UIPageControlTimerProgress

protocol UIPageControlTimerProgressDelegate

