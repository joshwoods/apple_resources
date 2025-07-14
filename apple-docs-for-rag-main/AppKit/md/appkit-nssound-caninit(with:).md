

- AppKit
- NSSound
-  canInit(with:) 

Type Method

# canInit(with:)

Indicates whether the receiver can create an instance of itself from the data in a pasteboard.

macOS

``` source
class func canInit(with pasteboard: NSPasteboard) -> Bool
```

## Parameters 

`pasteboard`  

Pasteboard containing sound data.

## Return Value

true when the receiver can handle the data represented by `pasteboard`; false otherwise.

## Discussion

The NSSound method is used to find out whether the class can handle the data in `pasteboard`.

## See Also

### Related Documentation

Sound Programming Topics for Cocoa

### Creating Sounds

init?(contentsOfFile: String, byReference: Bool)

Initializes the receiver with the audio data located at a given filepath.

init?(contentsOf: URL, byReference: Bool)

Initializes the receiver with the audio data located at a given URL.

init?(data: Data)

Initializes the receiver with a given audio data.

init?(pasteboard: NSPasteboard)

Initializes the receiver with data from a pasteboard. The pasteboard should contain a type returned by NSSound. `NSSound` expects the data to have a proper magic number, sound header, and data for the formats it supports.

