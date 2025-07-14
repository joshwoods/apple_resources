

- SwiftUI
- EnvironmentValues
-  lineLimit 

Instance Property

# lineLimit

The maximum number of lines that text can occupy in a view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var lineLimit: Int? { get set }
```

## Discussion

The maximum number of lines is `1` if the value is less than `1`. If the value is `nil`, the text uses as many lines as required. The default is `nil`.

## See Also

### Limiting line count for multiline text

func lineLimit(_:)

Sets to a closed range the number of lines that text can occupy in this view.

func lineLimit(Int, reservesSpace: Bool) -> some View

Sets a limit for the number of lines text can occupy in this view.

