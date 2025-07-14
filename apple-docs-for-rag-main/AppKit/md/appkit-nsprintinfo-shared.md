

- AppKit
- NSPrintInfo
-  shared 

Type Property

# shared

The shared printing information object.

macOS

``` source
class var shared: NSPrintInfo { get set }
```

## Return Value

The shared printer information.

## See Also

### Creating the Printing Information Object

init(dictionary: [NSPrintInfo.AttributeKey : Any])

Returns a printing information object initialized with the parameters in the specified dictionary.

convenience init()

Creates a printing information object.

init(coder: NSCoder)

Creates a printing information object from data in an unarchiver.

