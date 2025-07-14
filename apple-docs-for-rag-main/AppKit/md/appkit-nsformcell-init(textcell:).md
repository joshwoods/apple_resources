

- AppKit
- NSFormCell
-  init(textCell:) 

Initializer

# init(textCell:)

Returns an `NSFormCell` object initialized with the specified title string.

macOS

``` source
@MainActor
init(textCell string: String?)
```

## Parameters 

`string`  

The title for the new form cell object.

## Return Value

An initialized `NSFormCell` object.

## Discussion

The contents of the cell’s editable text entry field are set to the empty string (`@""`). The font for both title and text is the user’s chosen system font in 12.0 point, and the text area is drawn with a bezel. This method is the designated initializer for the `NSFormCell` class.

## See Also

### Related Documentation

Form Programming Topics

