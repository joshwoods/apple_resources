

- AppKit
- NSTextList
-  init(coder:) 

Initializer

# init(coder:)

Initializes and returns a newly allocated text list item.

macOS 10.0+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

An instance of NSCoder.

## See Also

### Creating a text list

convenience init(markerFormat: NSTextList.MarkerFormat, options: Int)

Returns an initialized text list.

init(markerFormat: NSTextList.MarkerFormat, options: NSTextList.Options, startingItemNumber: Int)

Returns a new text list with the format, options, and starting item number you provide.

