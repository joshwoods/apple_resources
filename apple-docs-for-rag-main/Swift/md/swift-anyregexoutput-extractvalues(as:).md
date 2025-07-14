

- Swift
- AnyRegexOutput
-  extractValues(as:) 

Instance Method

# extractValues(as:)

Returns strongly-typed match output by converting this type-erased output to the specified type, if possible.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func extractValues(as outputType: Output.Type = Output.self) -> Output?
```

## Parameters 

`outputType`  

The expected output type.

## Return Value

The output, if the underlying value can be converted to `outputType`; otherwise, `nil`.

