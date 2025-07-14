

- Network
- NWParameters
- NWParameters.PrivacyContext
-  disableLogging() 

Instance Method

# disableLogging()

Disables system logging of connection activity.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func disableLogging()
```

## See Also

### Configuring Custom Privacy Settings

init(description: String)

Initializes a privacy context with a description string.

static let `default`: NWParameters.PrivacyContext

The privacy context that applies to all connections that do not use a custom context.

func flushCache()

Flushes all cached data, such as TLS session state, created by connections associated with the privacy context.

