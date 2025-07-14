

- UIKit
- UIKey
-  characters 

Instance Property

# characters

A string that represents the text value of the key combined with any active modifier keys.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+

``` source
@MainActor
var characters: String { get }
```

## Discussion

When the user holds one or more modifier keys, this property contains the modified characters according to the rules of the particular modifier keys. For example, if the user holds Shift while pressing a letter button on a Latin keyboard, this property contains a capital letter.

## See Also

### Getting key characters

var charactersIgnoringModifiers: String

A string that represents the text value of the key without modifier keys.

