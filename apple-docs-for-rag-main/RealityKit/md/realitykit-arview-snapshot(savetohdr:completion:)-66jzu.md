

- RealityKit
- ARView
-  snapshot(saveToHDR:completion:) 

Instance Method

# snapshot(saveToHDR:completion:)

Takes a screenshot.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
func snapshot(
    saveToHDR: Bool,
    completion: @escaping (ARView.Image?) -> Void
)
```

## See Also

### Taking a snapshot

func snapshot(saveToHDR: Bool, completion: (ARView.Image?) -> Void)

Takes a screenshot.

typealias Image

