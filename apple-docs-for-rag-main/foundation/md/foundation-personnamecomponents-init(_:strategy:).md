

- Foundation
- PersonNameComponents
-  init(\_:strategy:) 

Initializer

# init(\_:strategy:)

Creates a person name components object from a given string by applying the provided parsing strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ value: S.ParseInput,
    strategy: S
) throws where S : ParseStrategy, S.ParseOutput == PersonNameComponents
```

## Parameters 

`value`  

A string to parse into person name components.

`strategy`  

The strategy used to parse a string into person name components.

## Discussion

This method uses a combination of locale rules and the provided parse strategy object to determine the most likely name components for a particular string representation. Parsing name components from a representation created for an existing name components object may not produce equivalent results.

Important

The format style only parses names using Latin or CJK scripts.

## See Also

### Parsing Person Name Components

init(String) throws

Creates a person name components object from a given string.

