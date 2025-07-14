

- WebKit
- WebView
-  canMakeTextLarger 

Instance Property

# canMakeTextLarger

A Boolean that indicates whether the text can be made larger.

macOS

``` source
@MainActor
var canMakeTextLarger: Bool { get }
```

## Discussion

true if able to make the text larger; otherwise, false.

## See Also

### Changing the Text Size

func makeTextLarger(Any?)

Action method that increases the text size by one unit.

var canMakeTextSmaller: Bool

A Boolean that indicates whether the text can be made smaller.

func makeTextSmaller(Any?)

Action method that reduces the text size by one unit.

