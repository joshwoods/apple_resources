

- VisionKit
- RecognizedItem
- RecognizedItem.Text
-  id 

Instance Property

# id

A unique identifier for the recognized item.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
var id: UUID { get }
```

## Discussion

If the same item resides in more than one video frame, the `id` remains the same.

