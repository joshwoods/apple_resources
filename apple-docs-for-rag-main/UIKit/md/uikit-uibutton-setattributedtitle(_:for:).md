

- UIKit
- UIButton
-  setAttributedTitle(\_:for:) 

Instance Method

# setAttributedTitle(\_:for:)

Sets the styled title to use for the specified state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setAttributedTitle(
    _ title: NSAttributedString?,
    for state: UIControl.State
)
```

## Parameters 

`title`  

The styled text string so use for the title.

`state`  

The state that uses the specified title. The possible values are described in UIControl.State.

## Discussion

Use this method to set the title of the button, including any relevant formatting information. If you set both a title and an attributed title for the button, the button prefers the use of the attributed title.

At a minimum, you should set the value for the normal state. If a title is not specified for a state, the default behavior is to use the title associated with the normal state. If the value for normal is not set, then the property defaults to a system value.

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

func titleColor(for: UIControl.State) -> UIColor?

Returns the title color used for a state.

func setTitleColor(UIColor?, for: UIControl.State)

Sets the color of the title to use for the specified state.

func titleShadowColor(for: UIControl.State) -> UIColor?

Returns the shadow color of the title used for a state.

func setTitleShadowColor(UIColor?, for: UIControl.State)

Sets the color of the title shadow to use for the specified state.

