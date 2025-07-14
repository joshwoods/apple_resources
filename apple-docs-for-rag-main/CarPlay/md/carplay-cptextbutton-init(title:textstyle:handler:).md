

- CarPlay
- CPTextButton
-  init(title:textStyle:handler:) 

Initializer

# init(title:textStyle:handler:)

Creates a button that displays a title in a specific style.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init(
    title: String,
    textStyle: CPTextButtonStyle,
    handler: ((CPTextButton) -> Void)? = nil
)
```

## Parameters 

`title`  

The text that the button displays.

`textStyle`  

The style that the button applies to its title.

`handler`  

A closure that CarPlay invokes when the user taps the button.

