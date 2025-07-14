

- AppKit
- NSFilePromiseReceiver
-  fileNames 

Instance Property

# fileNames

An array containing names of the promised files being written to the destination location.

macOS 10.12+

``` source
var fileNames: [String] { get }
```

## Discussion

This property returns an empty array until the file promise is called using receivePromisedFiles(atDestination:options:operationQueue:reader:).

## See Also

### Instance Properties

var fileTypes: [String]

An array containing types of the promised files being written to the destination location.

