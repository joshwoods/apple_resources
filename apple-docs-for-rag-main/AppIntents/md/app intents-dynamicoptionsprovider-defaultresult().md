

- App Intents
- DynamicOptionsProvider
-  defaultResult() 

Instance Method

# defaultResult()

The default value for parameters using this provider when no value is provided by the user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func defaultResult() async -> Self.DefaultValue?
```

**Required** Default implementation provided.

## Discussion

Either a single value or an array of values may be provided. If an array is provided and the parameter requires a single value, only the first element of the array is used.

## Default Implementations

### DynamicOptionsProvider Implementations

func defaultResult() async -> Self.DefaultValue?

The default value for parameters using this provider when no value is provided by the user.

## See Also

### Returning the parameter options

func results() async throws -> Self.Result

**Required** Default implementation provided.

associatedtype Result : ResultsCollection

**Required**

