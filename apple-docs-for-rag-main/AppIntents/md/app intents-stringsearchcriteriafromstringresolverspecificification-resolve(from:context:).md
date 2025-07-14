

- App Intents
- StringSearchCriteriaFromStringResolverSpecificification
-  resolve(from:context:) 

Instance Method

# resolve(from:context:)

Converts the specified value into the expected data type.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
func resolve(
    from input: String,
    context: IntentParameterContext
) async throws -> StringSearchCriteria?
```

## Parameters 

`input`  

The value to convert.

`context`  

Contextual resolution information, including resolution source and information about the associated parameter if applicable.

## Return Value

The converted value, or `nil` if conversion fails.

