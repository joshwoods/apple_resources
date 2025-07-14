

- RealityKit
- Entity
- Entity.ConfigurationCatalog
- Entity.ConfigurationCatalog.ConfigurationSet
-  configurations 

Instance Property

# configurations

The alternative configurations that are available in a set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var configurations: [String : Entity.ConfigurationCatalog.Configuration] { get }
```

## Discussion

The keys are configuration IDs, and the values are the corresponding configurations.

## See Also

### Accessing configurations in a configuration set

var defaultConfiguration: Entity.ConfigurationCatalog.Configuration

The default configuration, if you don’t explicitly set one.

