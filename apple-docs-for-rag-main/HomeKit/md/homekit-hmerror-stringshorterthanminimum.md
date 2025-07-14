

- HomeKit
- HMError
-  stringShorterThanMinimum 

Type Property

# stringShorterThanMinimum

An attempt to use a string shorter than the required minimum.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
static var stringShorterThanMinimum: HMError.Code { get }
```

## See Also

### Detecting value errors

static var invalidDataFormatSpecified: HMError.Code

An error indicating an invalid data format was specified.

static var invalidValueType: HMError.Code

An attempt to use an invalid value type.

static var nameContainsProhibitedCharacters: HMError.Code

An attempt to name an object with prohibited characters.

static var nameDoesNotEndWithValidCharacters: HMError.Code

An error indicating the provided name has invalid characters at the end.

static var nameDoesNotStartWithValidCharacters: HMError.Code

An attempt to start the name of an object with invalid characters.

static var stringLongerThanMaximum: HMError.Code

An attempt to use a string longer than the maximum allowed.

static var valueHigherThanMaximum: HMError.Code

An attempt to use a numeric value higher than the specified maximum value.

static var valueLowerThanMinimum: HMError.Code

An attempt to use a numeric value lower than the specified minimum value.

