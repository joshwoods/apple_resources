

- HomeKit
- HMError
- HMError.Code
-  HMError.Code.nameDoesNotStartWithValidCharacters 

Case

# HMError.Code.nameDoesNotStartWithValidCharacters

An attempt to start the name of an object with invalid characters.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
case nameDoesNotStartWithValidCharacters
```

## Discussion

Names must start with a letter, symbol, or number.

## See Also

### Value errors

case invalidDataFormatSpecified

An error indicating an invalid data format was specified.

case invalidValueType

An attempt to use an invalid value type.

case nameContainsProhibitedCharacters

An attempt to name an object with prohibited characters.

case nameDoesNotEndWithValidCharacters

An error indicating the provided name has invalid characters at the end.

case stringLongerThanMaximum

An attempt to use a string longer than the maximum allowed.

case stringShorterThanMinimum

An attempt to use a string shorter than the required minimum.

case valueHigherThanMaximum

An attempt to use a numeric value higher than the specified maximum value.

case valueLowerThanMinimum

An attempt to use a numeric value lower than the specified minimum value.

