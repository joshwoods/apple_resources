

- SwiftUI
- ProgressViewStyleConfiguration
-  label 

Instance Property

# label

A view that describes the task represented by the progress view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var label: ProgressViewStyleConfiguration.Label?
```

## Discussion

If `nil`, then the task is self-evident from the surrounding context, and the style does not need to provide any additional description.

If the progress view is defined using a `Progress` instance, then this label is equivalent to its `localizedDescription`.

## See Also

### Configuring the label

struct Label

A type-erased label describing the task represented by the progress view.

