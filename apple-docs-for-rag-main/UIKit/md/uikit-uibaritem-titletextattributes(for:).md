

- UIKit
- UIBarItem
-  titleTextAttributes(for:) 

Instance Method

# titleTextAttributes(for:)

Returns the title’s text attributes for a given control state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func titleTextAttributes(for state: UIControl.State) -> [NSAttributedString.Key : Any]?
```

## Parameters 

`state`  

The control state for which you want to know the text attributes for the title.

## Return Value

The title’s text attributes for `state`.

## Discussion

The dictionary may contain key-value pairs for text attributes for the font, text color, text shadow color, and text shadow offset using the keys listed in NSString UIKit Additions Reference.

## See Also

### Customizing appearance

func setTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the title’s text attributes for a given control state.

