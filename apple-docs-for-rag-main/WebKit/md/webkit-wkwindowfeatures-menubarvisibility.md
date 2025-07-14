

- WebKit
- WKWindowFeatures
-  menuBarVisibility 

Instance Property

# menuBarVisibility

A Boolean value that indicates whether the webpage requests a visible menu bar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var menuBarVisibility: NSNumber? { get }
```

## Discussion

If the webpage didn’t request a visible menu bar, this property is `nil`.

## See Also

### Inspecting Visibility Properties

var statusBarVisibility: NSNumber?

A Boolean value that indicates whether the webpage requested a visible status bar.

var toolbarsVisibility: NSNumber?

A Boolean value that indicates whether the webpage requested a visible toolbar.

