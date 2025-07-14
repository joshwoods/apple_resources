

- WatchKit
- WKInterfaceTextField
-  setPlaceholder(\_:) 

Instance Method

# setPlaceholder(\_:)

Sets the text field’s placeholder.

watchOS 6.0+

``` source
func setPlaceholder(_ placeholder: String?)
```

## Discussion

Use placeholders to describe the text field’s expected content to the user. An empty text field displays the placeholder, and any entered text hides the placeholder. The system automatically formats the placeholder, making it obvious that it’s not a valid text entry.

## See Also

### Setting a Placeholder

func setAttributedPlaceholder(NSAttributedString?)

Sets the text field’s placeholder using styled text.

