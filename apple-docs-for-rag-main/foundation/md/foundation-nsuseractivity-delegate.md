

- Foundation
- NSUserActivity
-  delegate 

Instance Property

# delegate

The user activity object’s delegate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any NSUserActivityDelegate)? { get set }
```

## Discussion

The user activity delegate is informed when the activity is being saved or continued. For more information on how to implement the delegate, see NSUserActivityDelegate.

## See Also

### Accessing the delegate

protocol NSUserActivityDelegate

The interface through which a user activity instance notifies its delegate of updates.

