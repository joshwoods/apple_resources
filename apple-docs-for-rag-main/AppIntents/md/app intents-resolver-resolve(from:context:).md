

- App Intents
- Resolver
-  resolve(from:context:) 

Instance Method

# resolve(from:context:)

Converts the specified value into the expected data type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func resolve(
    from input: Self.Input,
    context: IntentParameterContext
) async throws -> Self.Output?
```

**Required**

## Parameters 

`input`  

The value to convert.

`context`  

Contextual resolution information, including resolution source and information about the associated parameter if applicable.

## Return Value

The converted value, or `nil` if conversion fails.

## See Also

### Resolving the type

associatedtype Input : _IntentValue

**Required**

associatedtype Output : _IntentValue

**Required**

