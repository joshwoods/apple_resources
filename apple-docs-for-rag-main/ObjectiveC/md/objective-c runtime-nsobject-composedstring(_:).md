

- Objective-C Runtime
- NSObject
-  composedString(\_:) 

Instance Method

# composedString(\_:)

Return the current composed string.

macOS

``` source
func composedString(_ sender: Any!) -> Any!
```

## Parameters 

`sender`  

The client object requesting the string.

## Return Value

The current composed string, which can be an `NSString` or `NSAttributedString` object. The returned object should be an autoreleased object.

## Discussion

A composed string refers to the buffer that an input method typically maintains to mirror the text contained in the active inline area. It is called the composed string to reflect the fact that the input method composed the string by converting the characters input by the user. In addition, using the term composed string makes it easier to differentiate between an input method buffer and the text in the active inline area that the user sees.

