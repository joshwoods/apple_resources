

- App Intents
- DoubleFromIntResolver
-  resolve(from:context:) 

Instance Method

# resolve(from:context:)

Converts the specified value into the expected data type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func resolve(
    from input: Int,
    context: IntentParameterContext
) async throws -> Double?
```

## Parameters 

`input`  

The value to convert.

`context`  

Contextual resolution information, including resolution source and information about the associated parameter if applicable.

## Return Value

The converted value, or `nil` if conversion fails.

