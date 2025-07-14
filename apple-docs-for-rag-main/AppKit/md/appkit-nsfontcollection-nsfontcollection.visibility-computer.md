

- AppKit
- NSFontCollection
- NSFontCollection.Visibility
-  computer 

Type Property

# computer

The font collection is visible to all users and is stored persistently.

macOS

``` source
static var computer: NSFontCollection.Visibility { get }
```

## See Also

### Visibility Options

static var process: NSFontCollection.Visibility

The font collection is visible within this process and is not persistent.

static var user: NSFontCollection.Visibility

The font collection is visible to all processes and is stored persistently.

