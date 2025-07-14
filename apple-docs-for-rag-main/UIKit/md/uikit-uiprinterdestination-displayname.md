

- UIKit
- UIPrinterDestination
-  displayName 

Instance Property

# displayName

A human-readable string that displays the name of a printer.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var displayName: String? { get set }
```

## Discussion

This property contains a name that describes the printer’s manufacturer and model number to display in the app’s user interface. If `nil`, the txtRecord property can produce the display name.

## See Also

### Describing the printer

var txtRecord: Data?

A DNS TXT record to identify the printer.

var url: URL

The address of the printer.

