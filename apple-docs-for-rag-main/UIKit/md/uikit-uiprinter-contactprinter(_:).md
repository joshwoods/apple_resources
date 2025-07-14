

- UIKit
- UIPrinter
-  contactPrinter(\_:) 

Instance Method

# contactPrinter(\_:)

Connects to the printer and gathers information about its capabilities.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func contactPrinter(_ completionHandler: ((Bool) -> Void)? = nil)
```

``` source
@MainActor
func contactPrinter() async -> Bool
```

## Parameters 

`completionHandler`  

The block to execute with the results. This block has no return value and takes the following parameter:

available  
true if the printer was available and its information was retrieved or false if the printer could not be found or was unavailable.

## Discussion

For printers you create yourself using the init(url:) method, you must call this method prior to accessing properties containing printer-related information. This method runs asynchronously, returning immediately while the system continues to try and gather information about the printer’s name, location, capabilities, and so on. When the printer’s availability is determined, the results are delivered to the `completionHandler` block you provided.

Calling this method can take a significantly long time (up to 30 seconds), so after calling this method you should continue with other tasks. Use your completion handler block to update your app as appropriate.

