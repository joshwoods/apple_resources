

- XCTest
- XCTestObservationCenter
-  addTestObserver(\_:) 

Instance Method

# addTestObserver(\_:)

Registers an object conforming to XCTestObservation as an observer for the current test session.

``` source
func addTestObserver(_ testObserver: any XCTestObservation)
```

## Discussion

Observers may be added at any time, but will not receive events that occurred before they were registered. The observation center maintains a strong reference to observers.Events may be delivered to observers in any order. Given observers A and B, A may be notified of a test failure before or after B. Any ordering dependencies or serialization requirements must be managed by clients.

## See Also

### Managing Observers

func removeTestObserver(any XCTestObservation)

Unregisters an object conforming to XCTestObservation as an observer for the current test session.

