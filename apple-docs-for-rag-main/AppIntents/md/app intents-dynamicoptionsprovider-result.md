

- App Intents
- DynamicOptionsProvider
-  Result 

Associated Type

# Result

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype Result : ResultsCollection
```

**Required**

## See Also

### Returning the parameter options

func results() async throws -> Self.Result

**Required** Default implementation provided.

func defaultResult() async -> Self.DefaultValue?

The default value for parameters using this provider when no value is provided by the user.

**Required** Default implementation provided.

