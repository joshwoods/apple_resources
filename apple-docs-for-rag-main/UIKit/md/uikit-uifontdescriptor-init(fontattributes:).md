

- UIKit
- UIFontDescriptor
-  init(fontAttributes:) 

Initializer

# init(fontAttributes:)

Creates a font descriptor with the specified attributes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(fontAttributes attributes: [UIFontDescriptor.AttributeName : Any] = [:])
```

## Parameters 

`attributes`  

The attributes for the new font descriptor. If `nil`, the font descriptor’s attribute dictionary will be empty.

## Return Value

The new font descriptor.

## See Also

### Initializing a font descriptor

convenience init()

Creates a font descriptor.

init?(coder: NSCoder)

Creates a font descriptor from data in an unarchiver.

