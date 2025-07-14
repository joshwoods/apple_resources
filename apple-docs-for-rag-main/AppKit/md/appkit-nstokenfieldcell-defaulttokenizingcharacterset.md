

- AppKit
- NSTokenFieldCell
-  defaultTokenizingCharacterSet 

Type Property

# defaultTokenizingCharacterSet

Returns the default tokenizing character set.

macOS

``` source
@MainActor
class var defaultTokenizingCharacterSet: CharacterSet { get }
```

## Return Value

The default tokenizing character set.

## Discussion

The default tokenizing character set contains the single character “`,`”.

## See Also

### Managing the Tokenizing Character Set

var tokenizingCharacterSet: CharacterSet!

The receiver’s tokenizing character set to a given character set.

