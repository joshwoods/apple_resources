

- App Intents
- Resolver
-  Input 

Associated Type

# Input

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype Input : _IntentValue
```

**Required**

## See Also

### Resolving the type

func resolve(from: Self.Input, context: IntentParameterContext&lt;Self.Output>) async throws -> Self.Output?

Converts the specified value into the expected data type.

**Required**

associatedtype Output : _IntentValue

**Required**

