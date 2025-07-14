

- UIKit
- UIBarItem
-  setTitleTextAttributes(\_:for:) 

Instance Method

# setTitleTextAttributes(\_:for:)

Sets the title’s text attributes for a given control state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTitleTextAttributes(
    _ attributes: [NSAttributedString.Key : Any]?,
    for state: UIControl.State
)
```

## Parameters 

`attributes`  

A dictionary containing key-value pairs for text attributes.

You can specify the font, text color, text shadow color, and text shadow offset using the keys listed in NSString UIKit Additions Reference.

`state`  

The control state for which you want to set the text attributes for the title.

## See Also

### Customizing appearance

func titleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the title’s text attributes for a given control state.

