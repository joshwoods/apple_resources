

- Core Location
- CLLocationManager
-  delegate 

Instance Property

# delegate

The delegate object to receive update events.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any CLLocationManagerDelegate)? { get set }
```

## Discussion

In iOS, this property is declared as `nonatomic`. In macOS, it is declared as `atomic`.

## See Also

### Receiving data from location services

protocol CLLocationManagerDelegate

The methods you use to receive events from an associated location-manager object.

