

- Watch Connectivity
- WCSessionFile
-  metadata 

Instance Property

# metadata

A dictionary of additional information that was sent with the file.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var metadata: [String : Any]? { get }
```

## Discussion

The keys of the dictionary are strings. The values are property-list object types.

## See Also

### Getting the File Information

var fileURL: URL

The URL of the file that was received.

