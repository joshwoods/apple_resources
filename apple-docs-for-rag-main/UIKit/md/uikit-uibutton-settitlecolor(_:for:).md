

- UIKit
- UIButton
-  setTitleColor(\_:for:) 

Instance Method

# setTitleColor(\_:for:)

Sets the color of the title to use for the specified state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTitleColor(
    _ color: UIColor?,
    for state: UIControl.State
)
```

## Parameters 

`color`  

The color of the title to use for the specified state.

`state`  

The state that uses the specified color. The possible values are described in UIControl.State.

## Discussion

In general, if a property is not specified for a state, the default is to use the normal value. If the normal value is not set, then the property defaults to a system value. Therefore, at a minimum, you should set the value for the normal state.

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

func titleColor(for: UIControl.State) -> UIColor?

Returns the title color used for a state.

func titleShadowColor(for: UIControl.State) -> UIColor?

Returns the shadow color of the title used for a state.

func setTitleShadowColor(UIColor?, for: UIControl.State)

Sets the color of the title shadow to use for the specified state.

