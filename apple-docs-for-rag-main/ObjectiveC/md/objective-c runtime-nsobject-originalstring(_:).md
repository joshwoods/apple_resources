

- Objective-C Runtime
- NSObject
-  originalString(\_:) 

Instance Method

# originalString(\_:)

Return the string that consists of the precomposed Unicode characters.

macOS

``` source
func originalString(_ sender: Any!) -> NSAttributedString!
```

## Parameters 

`sender`  

The client object requesting the original string.

## Return Value

The original string of precomposed unicode characters. If an input method stores the original input text, it returns that text. The return value is an attributed string so that the input method can restore changes they made to the font, and other attributes, if necessary. The returned object should be an autoreleased object.

