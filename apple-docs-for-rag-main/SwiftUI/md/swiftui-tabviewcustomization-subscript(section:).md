

- SwiftUI
- TabViewCustomization
-  subscript(section:) 

Instance Subscript

# subscript(section:)

The customization of the section, identified by its customization identifier.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
subscript(section id: String) -> TabViewCustomization.SectionCustomization { get set }
```

## Overview

Section tab order can be read by subscripting with the tab section’s id:

```
let order = customization[section: "com.myApp.categories"].tabOrder
```

To reset the order of an individual section, use resetTabOrder(). To reset the order of all sections, use resetSectionOrder().

