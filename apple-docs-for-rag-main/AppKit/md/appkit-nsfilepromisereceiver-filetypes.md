

- AppKit
- NSFilePromiseReceiver
-  fileTypes 

Instance Property

# fileTypes

An array containing types of the promised files being written to the destination location.

macOS 10.12+

``` source
var fileTypes: [String] { get }
```

## Discussion

NSFilePromiseProvider promises one file type per item. The `count` of `fileTypes` should tell you the number of promised files in this item, but that’s not always guaranteed. Some legacy file promisers list each unique `fileType` only once.

## See Also

### Instance Properties

var fileNames: [String]

An array containing names of the promised files being written to the destination location.

