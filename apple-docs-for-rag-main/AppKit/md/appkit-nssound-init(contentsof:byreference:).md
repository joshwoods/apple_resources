

- AppKit
- NSSound
-  init(contentsOf:byReference:) 

Initializer

# init(contentsOf:byReference:)

Initializes the receiver with the audio data located at a given URL.

macOS

``` source
init?(
    contentsOf url: URL,
    byReference byRef: Bool
)
```

## Parameters 

`url`  

URL to the sound file with which the receiver is to be initialized.

`byRef`  

When true only the name of the sound is stored with the `NSSound` instance when archived using encode(with:); otherwise the audio data is archived along with the instance.

## Return Value

Initialized `NSSound` instance.

## See Also

### Creating Sounds

class func canInit(with: NSPasteboard) -> Bool

Indicates whether the receiver can create an instance of itself from the data in a pasteboard.

init?(contentsOfFile: String, byReference: Bool)

Initializes the receiver with the audio data located at a given filepath.

init?(data: Data)

Initializes the receiver with a given audio data.

init?(pasteboard: NSPasteboard)

Initializes the receiver with data from a pasteboard. The pasteboard should contain a type returned by NSSound. `NSSound` expects the data to have a proper magic number, sound header, and data for the formats it supports.

