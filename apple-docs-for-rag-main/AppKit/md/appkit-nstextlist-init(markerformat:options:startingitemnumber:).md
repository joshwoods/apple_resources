

- AppKit
- NSTextList
-  init(markerFormat:options:startingItemNumber:) 

Initializer

# init(markerFormat:options:startingItemNumber:)

Returns a new text list with the format, options, and starting item number you provide.

macOS 13.0+

``` source
init(
    markerFormat: NSTextList.MarkerFormat,
    options: NSTextList.Options = [],
    startingItemNumber: Int
)
```

## Parameters 

`markerFormat`  

One of the possible NSTextList.MarkerFormat formats.

`options`  

One or more of the possible NSTextList.Options options.

`startingItemNumber`  

An integer that represents the stating item number.

## See Also

### Creating a text list

init?(coder: NSCoder)

Initializes and returns a newly allocated text list item.

convenience init(markerFormat: NSTextList.MarkerFormat, options: Int)

Returns an initialized text list.

