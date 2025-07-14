

- Core Services
- Carbon Core
- Carbon Core Functions
-  UCTypeSelectFindItem(\_:\_:\_:\_:\_:\_:) 

Function

# UCTypeSelectFindItem(\_:\_:\_:\_:\_:\_:)

macOS 10.4+

``` source
func UCTypeSelectFindItem(
    _ ref: UCTypeSelectRef!,
    _ listSize: UInt32,
    _ listDataPtr: UnsafeMutableRawPointer!,
    _ refcon: UnsafeMutableRawPointer!,
    _ userUPP: IndexToUCStringUPP!,
    _ closestItem: UnsafeMutablePointer!
) -> OSStatus
```

