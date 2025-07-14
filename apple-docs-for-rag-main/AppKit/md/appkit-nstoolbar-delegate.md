

- AppKit
- NSToolbar
-  delegate 

Instance Property

# delegate

The object you use to customize the toolbar contents and configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
weak var delegate: (any NSToolbarDelegate)? { get set }
```

## Discussion

Assign an object to this property if you customize the toolbar’s behavior. The object you assign to this property must adopt the NSToolbarDelegate protocol.

## See Also

### Configuring the toolbar contents

protocol NSToolbarDelegate

A set of optional methods you use to configure the toolbar and respond to changes.

