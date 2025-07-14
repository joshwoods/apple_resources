

- Core Text
-  CTTypesetterCreateWithAttributedString(\_:) 

Function

# CTTypesetterCreateWithAttributedString(\_:)

Creates an immutable typesetter object using an attributed string.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTTypesetterCreateWithAttributedString(_ string: CFAttributedString) -> CTTypesetter
```

## Parameters 

`string`  

The attributed string to typeset. This parameter must be filled in with a valid CFAttributedString object.

## Return Value

A reference to a CTTypesetter object if the call was successful; otherwise, `NULL`.

## Discussion

The resultant typesetter can be used to create lines, perform line breaking, and do other contextual analysis based on the characters in the string.

## See Also

### Creating a Typesetter

func CTTypesetterCreateWithAttributedStringAndOptions(CFAttributedString, CFDictionary?) -> CTTypesetter?

Creates an immutable typesetter object using an attributed string and a dictionary of options.

