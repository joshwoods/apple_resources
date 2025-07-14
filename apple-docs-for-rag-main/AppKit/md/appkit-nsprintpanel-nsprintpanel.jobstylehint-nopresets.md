

- AppKit
- NSPrintPanel
- NSPrintPanel.JobStyleHint
-  noPresets 

Type Property

# noPresets

Output excludes all graphics printing.

macOS 10.6+

``` source
static let noPresets: NSPrintPanel.JobStyleHint
```

## Discussion

Equivalent to Core Printing’s `kPMPresetGraphicsTypeNone`.

## See Also

### Constants

static let photo: NSPrintPanel.JobStyleHint

Output contains photographic data.

static let allPresets: NSPrintPanel.JobStyleHint

Output appropriate to all graphics types.

