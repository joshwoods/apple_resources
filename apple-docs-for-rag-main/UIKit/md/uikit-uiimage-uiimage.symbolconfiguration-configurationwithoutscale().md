

- UIKit
- UIImage
- UIImage.SymbolConfiguration
-  configurationWithoutScale() 

Instance Method

# configurationWithoutScale()

Returns a copy of the current symbol configuration object without scale information.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func configurationWithoutScale() -> Self
```

## Return Value

A new symbol configuration object without the specified information.

## Discussion

This method sets the scale value in the new object to UIImage.SymbolScale.unspecified.

## See Also

### Removing configuration attributes

func configurationWithoutPointSizeAndWeight() -> Self

Returns a copy of the current symbol configuration object without point-size and weight information.

func configurationWithoutTextStyle() -> Self

Returns a copy of the current symbol configuration object without font text style information.

func configurationWithoutWeight() -> Self

Returns a copy of the current symbol configuration object without weight information.

