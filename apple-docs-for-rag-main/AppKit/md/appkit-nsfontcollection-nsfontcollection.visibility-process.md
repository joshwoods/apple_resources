

- AppKit
- NSFontCollection
- NSFontCollection.Visibility
-  process 

Type Property

# process

The font collection is visible within this process and is not persistent.

macOS

``` source
static var process: NSFontCollection.Visibility { get }
```

## See Also

### Visibility Options

static var user: NSFontCollection.Visibility

The font collection is visible to all processes and is stored persistently.

static var computer: NSFontCollection.Visibility

The font collection is visible to all users and is stored persistently.

