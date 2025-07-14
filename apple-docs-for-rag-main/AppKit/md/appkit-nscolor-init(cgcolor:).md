

- AppKit
- NSColor
-  init(cgColor:) 

Initializer

# init(cgColor:)

Creates a color object using the specified Core Graphics color.

macOS 10.8+

``` source
init?(cgColor: CGColor)
```

## Parameters 

`cgColor`  

The Core Graphics color reference.

## Return Value

An `NSColor` instance.

## Discussion

This method may return `nil`.

## See Also

### Converting Other Types of Color Objects

convenience init(Color)

init(CIColor: CIColor)

Creates a color object from the specified Core Image color.

