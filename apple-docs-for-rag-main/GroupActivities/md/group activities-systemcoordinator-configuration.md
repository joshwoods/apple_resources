

- Group Activities
- SystemCoordinator
-  configuration 

Instance Property

# configuration

The current configuration of the system coordinator.

visionOS 1.0+

``` source
final var configuration: SystemCoordinator.Configuration { get set }
```

## Discussion

This property stores the SystemCoordinator object’s current support for displaying spatial Personas and placing them and your content in a shared simulation space. Assign a new value to this property to support spatial Personas and shared context in the current activity. The default configuration doesn’t enable support for these features.

## See Also

### Configuring the system coordinator

struct Configuration

A structure that specifies your app’s support for activities that take place in a shared simulation space.

