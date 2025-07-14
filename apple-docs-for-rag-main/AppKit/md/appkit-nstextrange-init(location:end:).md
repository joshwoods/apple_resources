

- AppKit
- NSTextRange
-  init(location:end:) 

Initializer

# init(location:end:)

Creates a new text range with the starting and ending locations you specify.

macOS 12.0+

``` source
init?(
    location: any NSTextLocation,
    end endLocation: (any NSTextLocation)?
)
```

## Parameters 

`location`  

The starting location.

`endLocation`  

The ending location.

## See Also

### Creating a text range

convenience init(location: any NSTextLocation)

Creates a new text range at the location you specify.

