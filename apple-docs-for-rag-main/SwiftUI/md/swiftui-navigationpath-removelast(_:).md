

- SwiftUI
- NavigationPath
-  removeLast(\_:) 

Instance Method

# removeLast(\_:)

Removes values from the end of this path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func removeLast(_ k: Int = 1)
```

## Parameters 

`k`  

The number of values to remove. The default value is `1`.

## Discussion

Precondition

The input parameter `k` must be greater than or equal to zero, and must be less than or equal to the number of elements in the path.

## See Also

### Managing path contents

var isEmpty: Bool

A Boolean that indicates whether this path is empty.

var count: Int

The number of elements in this path.

func append(_:)

Appends a new codable value to the end of this path.

