

- RealityKit
- ARView
- 
  - ARView
- ARView.Environment
- ARView.Environment.SceneUnderstanding
- ARView.Environment.SceneUnderstanding.Options
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15+

``` source
let rawValue: UInt32
```

## Discussion

A new instance initialized with `rawValue` will be equivalent to this instance. For example:

```
enum PaperSize: String {
    case A4, A5, Letter, Legal
}

let selectedSize = PaperSize.Letter
print(selectedSize.rawValue)
// Prints "Letter"

print(selectedSize == PaperSize(rawValue: selectedSize.rawValue)!)
// Prints "true"
```

