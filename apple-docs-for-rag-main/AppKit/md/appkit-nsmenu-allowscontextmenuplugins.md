

- AppKit
- NSMenu
-  allowsContextMenuPlugIns 

Instance Property

# allowsContextMenuPlugIns

Indicates whether the pop-up menu allows appending of contextual menu plug-in items.

macOS 10.6+

``` source
var allowsContextMenuPlugIns: Bool { get set }
```

## Discussion

This property contains a Boolean value indicating whether the pop-up menu allows appending of contextual menu plug-in items.

Contextual menu plug-ins are system-wide services provided by other applications. For example, a contextual menu plug-in might provide an “Open URL…” service. If you enable context menu plug-ins, your application’s contextual menu will display the appropriate items for the currently selected data type.

The default value for this property is true.

See Services Implementation Guide for more information on contextual menu plug-ins.

