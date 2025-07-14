

- UIKit
- UIStackView
-  setCustomSpacing(\_:after:) 

Instance Method

# setCustomSpacing(\_:after:)

Applies custom spacing after the specified view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func setCustomSpacing(
    _ spacing: CGFloat,
    after arrangedSubview: UIView
)
```

## See Also

### Adding space between items

func customSpacing(after: UIView) -> CGFloat

Returns the custom spacing after the specified view.

class let spacingUseDefault: CGFloat

The default spacing for subviews within a stack view.

class let spacingUseSystem: CGFloat

The system-defined spacing to the neighboring view.

