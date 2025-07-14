

- AppKit
- NSWorkspace
- NSWorkspace.OpenConfiguration
-  requiresUniversalLinks 

Instance Property

# requiresUniversalLinks

A Boolean value indicating whether you require the URL to have an associated universal link.

macOS 10.15+

``` source
var requiresUniversalLinks: Bool { get set }
```

## Discussion

The default value of this property is false, which tells the app to open any URL you provide. Set the value to true when you want the app to open only valid universal links.

The app must be specifically configured to open universal links, and attempts to open such links fail with an appropriate error if the app isn’t properly configured. Attempts may also fail with an error if the user disabled support for opening links with the specified app.

## See Also

### Handling URLs

var isForPrinting: Bool

A Boolean value indicating whether you want to print the contents of documents and URLs instead of opening them.

var isForPrinting: Bool

A Boolean value indicating whether you want to print the contents of documents and URLs instead of opening them.

