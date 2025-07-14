

- WatchKit
- WKInterfaceTextField
-  setAttributedPlaceholder(\_:) 

Instance Method

# setAttributedPlaceholder(\_:)

Sets the text field’s placeholder using styled text.

watchOS 6.0+

``` source
func setAttributedPlaceholder(_ attributedPlaceholder: NSAttributedString?)
```

## Discussion

Use placeholders to describe the text field’s expected content to the user. An empty text field displays the placeholder, and any entered text hides the placeholder. The system automatically formats the placeholder, making it obvious that it’s not a valid text entry.

## See Also

### Setting a Placeholder

func setPlaceholder(String?)

Sets the text field’s placeholder.

