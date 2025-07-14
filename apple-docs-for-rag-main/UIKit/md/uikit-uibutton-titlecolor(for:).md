

- UIKit
- UIButton
-  titleColor(for:) 

Instance Method

# titleColor(for:)

Returns the title color used for a state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func titleColor(for state: UIControl.State) -> UIColor?
```

## Parameters 

`state`  

The state that uses the title color. The possible values are described in UIControl.State.

## Return Value

The color of the title for the specified state.

## See Also

### Managing the title

var titleLabel: UILabel?

A view that displays the value of the `currentTitle` property for a button.

func title(for: UIControl.State) -> String?

Returns the title associated with the specified state.

func setTitle(String?, for: UIControl.State)

Sets the title to use for the specified state.

func attributedTitle(for: UIControl.State) -> NSAttributedString?

Returns the styled title associated with the specified state.

func setAttributedTitle(NSAttributedString?, for: UIControl.State)

Sets the styled title to use for the specified state.

func setTitleColor(UIColor?, for: UIControl.State)

Sets the color of the title to use for the specified state.

func titleShadowColor(for: UIControl.State) -> UIColor?

Returns the shadow color of the title used for a state.

func setTitleShadowColor(UIColor?, for: UIControl.State)

Sets the color of the title shadow to use for the specified state.

