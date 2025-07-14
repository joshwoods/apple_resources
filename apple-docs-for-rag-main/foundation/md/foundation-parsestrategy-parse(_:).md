

- Foundation
- ParseStrategy
-  parse(\_:) 

Instance Method

# parse(\_:)

Parses a value, using this strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func parse(_ value: Self.ParseInput) throws -> Self.ParseOutput
```

**Required**

## Parameters 

`value`  

A value whose type matches the strategy’s ParseInput type.

## Return Value

A parsed value of the type declared by ParseOutput.

## Discussion

This method throws an error if the parse strategy can’t parse `value`.

