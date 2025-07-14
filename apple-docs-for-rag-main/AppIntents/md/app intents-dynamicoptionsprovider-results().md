

- App Intents
- DynamicOptionsProvider
-  results() 

Instance Method

# results()

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func results() async throws -> Self.Result
```

**Required** Default implementation provided.

## Default Implementations

### DynamicOptionsProvider Implementations

func results() async throws -> Self.Result

## See Also

### Returning the parameter options

func defaultResult() async -> Self.DefaultValue?

The default value for parameters using this provider when no value is provided by the user.

**Required** Default implementation provided.

associatedtype Result : ResultsCollection

**Required**

