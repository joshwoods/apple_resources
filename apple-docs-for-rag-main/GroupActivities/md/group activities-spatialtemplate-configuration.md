

- Group Activities
- SpatialTemplate
-  configuration 

Instance Property

# configuration

Information a spatial template uses to configure itself.

visionOS 2.0+

``` source
var configuration: SpatialTemplateConfiguration { get }
```

**Required** Default implementation provided.

## Discussion

If you don’t specify a custom configuration at initialization time, the system provides one automatically.

## Default Implementations

### SpatialTemplate Implementations

var configuration: SpatialTemplateConfiguration

Information a spatial template uses to configure itself.

## See Also

### Configuring the spatial template

struct SpatialTemplateConfiguration

A type that contains the configuration details for a spatial template.

