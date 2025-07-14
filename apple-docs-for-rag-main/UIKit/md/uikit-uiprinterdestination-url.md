

- UIKit
- UIPrinterDestination
-  url 

Instance Property

# url

The address of the printer.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var url: URL { get set }
```

## Discussion

This property locates the IP address and resource path for the printer.

## See Also

### Describing the printer

var displayName: String?

A human-readable string that displays the name of a printer.

var txtRecord: Data?

A DNS TXT record to identify the printer.

