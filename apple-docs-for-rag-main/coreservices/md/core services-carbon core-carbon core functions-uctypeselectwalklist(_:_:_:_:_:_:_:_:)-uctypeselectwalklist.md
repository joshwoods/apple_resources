

- Core Services
- Carbon Core
- Carbon Core Functions
-  UCTypeSelectWalkList(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# UCTypeSelectWalkList(\_:\_:\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func UCTypeSelectWalkList(
    _ ref: UCTypeSelectRef!,
    _ currSelect: CFString!,
    _ direction: UCTSWalkDirection,
    _ listSize: UInt32,
    _ listDataPtr: UnsafeMutableRawPointer!,
    _ refcon: UnsafeMutableRawPointer!,
    _ userUPP: IndexToUCStringUPP!,
    _ closestItem: UnsafeMutablePointer!
) -> OSStatus
```

