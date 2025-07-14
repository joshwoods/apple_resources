

- AppKit
- NSGraphicsContext
- NSGraphicsContext.AttributeKey
-  destination 

Type Property

# destination

Specifies the destination.

macOS

``` source
static let destination: NSGraphicsContext.AttributeKey
```

## Discussion

This value can be an instance of NSWindow or NSBitmapImageRep when creating a graphics context.

When determining the type of a graphics context, this value can be an NSMutableData, NSString, or NSURL object.

## See Also

### Attribute Keys

static let representationFormat: NSGraphicsContext.AttributeKey

Specifies the destination file format.

