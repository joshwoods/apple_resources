

- SwiftUI
- TabViewCustomization
-  subscript(tab:) 

Instance Subscript

# subscript(tab:)

The customization of the tab, identified by its customization identifier.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
subscript(tab id: String) -> TabViewCustomization.TabCustomization { get set }
```

## Overview

You can imperatively set properties by subscripting with the tab ID. The following example sets the tab’s sidebar visibility:

```
customization[tab: "com.myApp.alerts"].sidebarVisibility = .hidden
```

