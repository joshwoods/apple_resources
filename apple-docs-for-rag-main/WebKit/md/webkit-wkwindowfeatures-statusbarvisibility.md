

- WebKit
- WKWindowFeatures
-  statusBarVisibility 

Instance Property

# statusBarVisibility

A Boolean value that indicates whether the webpage requested a visible status bar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var statusBarVisibility: NSNumber? { get }
```

## Discussion

If the webpage didn’t request a visible status bar, this property is `nil`.

## See Also

### Inspecting Visibility Properties

var menuBarVisibility: NSNumber?

A Boolean value that indicates whether the webpage requests a visible menu bar.

var toolbarsVisibility: NSNumber?

A Boolean value that indicates whether the webpage requested a visible toolbar.

