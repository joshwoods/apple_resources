

- Watch Connectivity
- WCSessionFile
-  fileURL 

Instance Property

# fileURL

The URL of the file that was received.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var fileURL: URL { get }
```

## Discussion

The system places downloaded files inside a temporary directory. If you intend to keep the file, it is your responsibility to move the file to a more permanent location inside your extension’s container directory. You must move the file before your session delegate’s session(_:didReceive:) method returns.

## See Also

### Getting the File Information

var metadata: [String : Any]?

A dictionary of additional information that was sent with the file.

