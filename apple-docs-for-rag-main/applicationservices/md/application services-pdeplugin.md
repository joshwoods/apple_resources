

- Application Services
-  PDEPlugIn 

Protocol

# PDEPlugIn

macOS 13.0+

``` source
protocol PDEPlugIn
```

## Topics

### Initializers

init?(bundle: Bundle)

**Required**

### Instance Methods

func pdePanels(forType: String, withHostInfo: any PDEPlugInCallbackProtocol) -> [any PDEPanel]?

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

