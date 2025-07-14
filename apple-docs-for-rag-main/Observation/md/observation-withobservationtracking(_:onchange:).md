

- Observation
-  withObservationTracking(\_:onChange:) 

Function

# withObservationTracking(\_:onChange:)

Tracks access to properties.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func withObservationTracking(
    _ apply: () -> T,
    onChange: @autoclosure () -> () -> Void
) -> T
```

## Parameters 

`apply`  

A closure that contains properties to track.

`onChange`  

The closure invoked when the value of a property changes.

## Return Value

The value that the `apply` closure returns if it has a return value; otherwise, there is no return value.

## Discussion

This method tracks access to any property within the `apply` closure, and informs the caller of value changes made to participating properties by way of the `onChange` closure. For example, the following code tracks changes to the name of cars, but it doesn’t track changes to any other property of `Car`:

```
func render() {
    withObservationTracking {
        for car in cars {
            print(car.name)
        }
    } onChange: {
        print("Schedule renderer.")
    }
}
```

## See Also

### Change tracking

struct ObservationRegistrar

Provides storage for tracking and access to data changes.

