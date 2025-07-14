

- Network
- NWParameters
- NWParameters.PrivacyContext
-  init(description:) 

Initializer

# init(description:)

Initializes a privacy context with a description string.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(description: String)
```

## See Also

### Configuring Custom Privacy Settings

static let `default`: NWParameters.PrivacyContext

The privacy context that applies to all connections that do not use a custom context.

func disableLogging()

Disables system logging of connection activity.

func flushCache()

Flushes all cached data, such as TLS session state, created by connections associated with the privacy context.

