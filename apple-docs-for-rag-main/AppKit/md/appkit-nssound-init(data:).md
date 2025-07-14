

- AppKit
- NSSound
-  init(data:) 

Initializer

# init(data:)

Initializes the receiver with a given audio data.

macOS

``` source
init?(data: Data)
```

## Parameters 

`data`  

Audio data with which the receiver is to be initialized. The data must have a proper magic number, sound header, and data for the formats the `NSSound` class supports.

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

init?(pasteboard: NSPasteboard)

Initializes the receiver with data from a pasteboard. The pasteboard should contain a type returned by NSSound. `NSSound` expects the data to have a proper magic number, sound header, and data for the formats it supports.

