

- TVMLKit JS
- Keyboard
-  onTextChange 

Instance Property

# onTextChange

A function the system calls when the text in a search or text field changes.

tvOS 9.0+

``` source
attribute function onTextChange;
```

## Discussion

Provide a callback function for the `onTextChange` attribute to respond to changes in the `searchField` or `textField` elements. You can respond to user inputs as the changes happen. This attribute must be set to a function; for example, `Keyboard.onTextChange = function () {}`.

## See Also

### Setting and Retrieving Text

text

The text inside a search or text field.

