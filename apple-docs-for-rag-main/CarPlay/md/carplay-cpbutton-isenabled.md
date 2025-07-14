

- CarPlay
- CPButton
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that determines whether the button is in an enabled state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

When false, CarPlay doesn’t call the button’s handler, and it changes the button’s appearance to reflect its disabled state.

The default value is true.

## See Also

### Configuring the Button’s Attributes

var title: String?

The button’s title.

