

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  isForPrinting 

Instance Property

# isForPrinting

A Boolean value indicating whether you want to print the contents of documents and URLs instead of opening them.

macOS 10.15+

``` source
var isForPrinting: Bool { get set }
```

## Discussion

The default value of this property is false, which causes the app to open documents and URLs. Set the value to true if you want the app to print the items instead.

## See Also

### Handling URLs

var requiresUniversalLinks: Bool

A Boolean value indicating whether you require the URL to have an associated universal link.

var requiresUniversalLinks: Bool

A Boolean value indicating whether you require the URL to have an associated universal link.

