

- AppKit
- NSSound
-  init(pasteboard:) 

Initializer

# init(pasteboard:)

Initializes the receiver with data from a pasteboard. The pasteboard should contain a type returned by NSSound. `NSSound` expects the data to have a proper magic number, sound header, and data for the formats it supports.

macOS

``` source
init?(pasteboard: NSPasteboard)
```

## Parameters 

`pasteboard`  

The pasteboard containing the audio data with which the receiver is to be initialized. The pasteboard must contain a type returned by NSSound. The contained data must have a proper magic number, sound header, and data for the formats the `NSSound` class supports.

## Return Value

Initialized `NSSound` instance.

## See Also

### Creating Sounds

class func canInit(with: NSPasteboard) -> Bool

Indicates whether the receiver can create an instance of itself from the data in a pasteboard.

init?(contentsOfFile: String, byReference: Bool)

Initializes the receiver with the audio data located at a given filepath.

init?(contentsOf: URL, byReference: Bool)

Initializes the receiver with the audio data located at a given URL.

init?(data: Data)

Initializes the receiver with a given audio data.

