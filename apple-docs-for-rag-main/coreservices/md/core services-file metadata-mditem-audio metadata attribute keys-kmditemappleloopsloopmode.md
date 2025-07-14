

- Core Services
- File Metadata
- MDItem
- Audio Metadata Attribute Keys
-  kMDItemAppleLoopsLoopMode 

Global Variable

# kMDItemAppleLoopsLoopMode

Specifies how a file should be played. A CFString.

macOS 10.4+

``` source
let kMDItemAppleLoopsLoopMode: CFString!
```

## Discussion

Tagged files can either be loops or non-loops (e.g., a cymbal crash). "Looping" indicates if the file should be treated as a loop. "Non-looping" indicates the file should not be treated as a loop.

