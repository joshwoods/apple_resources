

- UIKit
- UIButton
-  attributedTitle(for:) 

Instance Method

# attributedTitle(for:)

Returns the styled title associated with the specified state.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func attributedTitle(for state: UIControl.State) -> NSAttributedString?
```

## Parameters 

`state`  

The state that uses the styled title. The possible values are described in UIControl.State.

## Return Value

The title for the specified state. If no attributed title has been set for the specific state, this method returns the attributed title associated with the normal state. If no attributed title has been set for normal, returns `nil`.

## See Also

### Managing the title

var titleLabel: UILabel?

A view that displays the value of the `currentTitle` property for a button.

func title(for: UIControl.State) -> String?

Returns the title associated with the specified state.

func setTitle(String?, for: UIControl.State)

Sets the title to use for the specified state.

func setAttributedTitle(NSAttributedString?, for: UIControl.State)

Sets the styled title to use for the specified state.

func titleColor(for: UIControl.State) -> UIColor?

Returns the title color used for a state.

func setTitleColor(UIColor?, for: UIControl.State)

Sets the color of the title to use for the specified state.

func titleShadowColor(for: UIControl.State) -> UIColor?

Returns the shadow color of the title used for a state.

func setTitleShadowColor(UIColor?, for: UIControl.State)

Sets the color of the title shadow to use for the specified state.

