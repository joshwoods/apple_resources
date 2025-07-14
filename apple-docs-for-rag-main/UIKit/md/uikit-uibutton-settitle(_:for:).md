

- UIKit
- UIButton
-  setTitle(\_:for:) 

Instance Method

# setTitle(\_:for:)

Sets the title to use for the specified state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTitle(
    _ title: String?,
    for state: UIControl.State
)
```

## Parameters 

`title`  

The title to use for the specified state.

`state`  

The state that uses the specified title. UIControl.State describes the possible values.

## Discussion

Use this method to set the title for the button. The title you specify derives its formatting from the button’s associated label object. If you set both a title and an attributed title for the button, the button prefers the use of the attributed title over this one.

At a minimum, set the value for the normal state. If you don’t specify a title for the other states, the button uses the title associated with the normal state. If you don’t set the value for normal, then the property defaults to a system value.

Important

When the user interface idiom is UIUserInterfaceIdiom.mac and behavioralStyle is UIBehavioralStyle.mac, your app throws an exception if you use this method to set the title for any state other than normal.

## See Also

### Managing the title

var titleLabel: UILabel?

A view that displays the value of the `currentTitle` property for a button.

func title(for: UIControl.State) -> String?

Returns the title associated with the specified state.

func attributedTitle(for: UIControl.State) -> NSAttributedString?

Returns the styled title associated with the specified state.

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

