

- AppKit
- NSColor
-  init(CIColor:) 

Initializer

# init(CIColor:)

Creates a color object from the specified Core Image color.

macOS

``` source
init(CIColor color: CIColor)
```

``` source
init(ciColor color: CIColor)
```

## Parameters 

`color`  

The Core Image color to convert.

## Return Value

The `NSColor` object corresponding to the specified Core Image color.

## Discussion

The method raises if the color space and components associated with `color` are `nil` or invalid.

## See Also

### Converting Other Types of Color Objects

convenience init(Color)

init?(cgColor: CGColor)

Creates a color object using the specified Core Graphics color.

