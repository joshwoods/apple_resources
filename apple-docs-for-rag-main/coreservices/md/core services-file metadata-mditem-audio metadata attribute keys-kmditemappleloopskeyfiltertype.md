

- Core Services
- File Metadata
- MDItem
- Audio Metadata Attribute Keys
-  kMDItemAppleLoopsKeyFilterType 

Global Variable

# kMDItemAppleLoopsKeyFilterType

Specifies key filtering information about a loop. Loops are matched against projects that often in a major or minor key. A CFString.

macOS 10.4+

``` source
let kMDItemAppleLoopsKeyFilterType: CFString!
```

## Discussion

To assist users in identifying loops that will "fit" with their compositions, loops can be tagged with one of the following key filters: "AnyKey" "Minor" "Major" "NeitherKey" "BothKeys". "AnyKey" means that it fits with anything (whether in a major key, minor key or neither). "Minor" fits with compositions in a minor key. "NeitherKey" doesn't work well with compositions that are in major or minor key. "BothKeys" means it fits with major or minor key.

