

- SwiftUI
- TableColumnCustomization
-  subscript(visibility:) 

Instance Subscript

# subscript(visibility:)

The visibility of the column identified by its identifier.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
subscript(visibility id: String) -> Visibility { get set }
```

## Overview

Explicit identifiers can be associated with a `TableColumn` using the `customizationID(_:)` modifier.

```
TableColumn("Number of Reports", value: \.duplicateCount) {
    Text($0.duplicateCount, format: .number)
}
.customizationID("numberOfReports")

...

columnsCustomization[visibility: "numberOfReports"] = .hidden
```

If the ID isn’t associated with the state, a default value of `.automatic` is returned.

## See Also

### Managing the customization

func resetOrder()

Resets the column order back to the default, preserving the customized visibility and size.

