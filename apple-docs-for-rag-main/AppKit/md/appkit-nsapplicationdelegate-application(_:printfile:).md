

- AppKit
- NSApplicationDelegate
-  application(\_:printFile:) 

Instance Method

# application(\_:printFile:)

Returns a Boolean value that indicates if the app prints the specified file in its entirety.

macOS

``` source
@MainActor
optional func application(
    _ sender: NSApplication,
    printFile filename: String
) -> Bool
```

## Parameters 

`sender`  

The application object that is handling the printing.

`filename`  

The name of the file to print.

## Return Value

true if the file was successfully printed or false if it was not.

## Discussion

This message is sent directly by `theApplication` to the delegate. The application terminates (using the terminate(_:) method) after this method returns.

If at all possible, this method should print the file without displaying the user interface. For example, if you pass the `-NSPrint` option to the TextEdit application, TextEdit assumes you want to print the entire contents of the specified file. However, if the application opens more complex documents, you may want to display a panel that lets the user choose exactly what they want to print.

## See Also

### Related Documentation

func application(Any, openFileWithoutUI: String) -> Bool

Returns a Boolean value that indicates if the app opens the specified file without showing its user interface.

### Printing

func application(NSApplication, printFiles: [String], withSettings: [NSPrintInfo.AttributeKey : Any], showPrintPanels: Bool) -> NSApplication.PrintReply

Returns a value that indicates if the app prints the specified files.

enum PrintReply

Constants that indicate the outcome of a print request.

