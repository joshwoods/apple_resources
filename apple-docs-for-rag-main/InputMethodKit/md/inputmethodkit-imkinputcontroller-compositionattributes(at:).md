

- InputMethodKit
- IMKInputController
-  compositionAttributes(at:) 

Instance Method

# compositionAttributes(at:)

Returns a dictionary of text attributes.

macOS 10.5+

``` source
func compositionAttributes(at range: NSRange) -> NSMutableDictionary!
```

## Parameters 

`range`  

The range of text whose attributes you want to obtain.

## Return Value

The dictionary of text attributes. The default implementation returns an empty dictionary.

## See Also

### Working with Ranges

func selectionRange() -> NSRange

Returns where the range of the selection that should be placed inside marked text.

func replacementRange() -> NSRange

Returns the range in the client document that the text should replace.

func mark(forStyle: Int, at: NSRange) -> [AnyHashable : Any]!

Returns a dictionary of text attributes that can mark a range of an attributed string to send to a client.

