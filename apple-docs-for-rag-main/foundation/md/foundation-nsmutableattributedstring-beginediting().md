

- Foundation
- NSMutableAttributedString
-  beginEditing() 

Instance Method

# beginEditing()

Begins the buffering of changes to the string’s characters and attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func beginEditing()
```

## Discussion

Override this method in a subclass to buffer or optimize a series of changes to the string’s characters or attributes. The string continues to buffer text until you call endEditing(), at which time it consolidates the changes and notifies observers.

You can nest pairs of beginEditing() and endEditing() messages.

## See Also

### Grouping Changes

func endEditing()

Ends the buffering of changes to the string’s characters and attributes.

