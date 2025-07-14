

- Game Controller
- GCControllerElement
-  unmappedSfSymbolsName 

Instance Property

# unmappedSfSymbolsName

The element’s system symbol, not the remapped symbol.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var unmappedSfSymbolsName: String? { get set }
```

## Discussion

Use this property to get the original unmapped name. Otherwise, use the sfSymbolsName property to get the possibly remapped symbol.

## See Also

### Displaying a symbol

var sfSymbolsName: String?

A system symbol for the element or the remapped element.

