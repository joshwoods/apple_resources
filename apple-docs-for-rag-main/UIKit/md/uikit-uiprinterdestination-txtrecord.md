

- UIKit
- UIPrinterDestination
-  txtRecord 

Instance Property

# txtRecord

A DNS TXT record to identify the printer.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var txtRecord: Data? { get set }
```

## Discussion

This property supplies additional information about a printing service as a set of strings that the system can parse into a series of key/value pairs. The TXT record can provide basic access, identity, and capability information about the printing service. The interface can then locate the printer based on categories such as color or duplex printing.

A TXT record isn’t required. When absent, the print system queries the URL and verifies that it can reach the printer before presenting it to the user.

## See Also

### Describing the printer

var displayName: String?

A human-readable string that displays the name of a printer.

var url: URL

The address of the printer.

