

- Audio Toolbox
- AudioComponentPlugInInterface
-  init(Open:Close:Lookup:reserved:) 

Initializer

# init(Open:Close:Lookup:reserved:)

macOS

``` source
init(
    Open: (UnsafeMutableRawPointer, AudioComponentInstance) -> OSStatus,
    Close: (UnsafeMutableRawPointer) -> OSStatus,
    Lookup: (Int16) -> AudioComponentMethod?,
    reserved: UnsafeMutableRawPointer?
)
```

