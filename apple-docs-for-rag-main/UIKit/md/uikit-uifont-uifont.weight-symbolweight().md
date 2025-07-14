

- UIKit
- UIFont
- UIFont.Weight
-  symbolWeight() 

Instance Method

# symbolWeight()

Provides the corresponding symbol weight for this font weight.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func symbolWeight() -> UIImage.SymbolWeight
```

## Return Value

The UIImage.SymbolWeight that most closely coordinates with the provided font weight.

## Discussion

When placing symbols adjacent to text, use this method to find the appropriate symbol weight to match the weight of the text. Similarly, if you want to display a symbol with a particular weight, you can use fontWeight() to look up the matching font weight for adjacent text.

