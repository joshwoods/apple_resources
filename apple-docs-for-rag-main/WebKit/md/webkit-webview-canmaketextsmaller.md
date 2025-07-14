

- WebKit
- WebView
-  canMakeTextSmaller 

Instance Property

# canMakeTextSmaller

A Boolean that indicates whether the text can be made smaller.

macOS

``` source
@MainActor
var canMakeTextSmaller: Bool { get }
```

## Discussion

true if able to make the text smaller; otherwise, false.

## See Also

### Changing the Text Size

var canMakeTextLarger: Bool

A Boolean that indicates whether the text can be made larger.

func makeTextLarger(Any?)

Action method that increases the text size by one unit.

func makeTextSmaller(Any?)

Action method that reduces the text size by one unit.

