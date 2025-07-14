

- SwiftUI
- NavigationPath
-  append(\_:) 

Instance Method

# append(\_:)

Appends a new codable value to the end of this path.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
mutating func append(_ value: V) where V : Decodable, V : Encodable, V : Hashable
```

Show all declarations

## See Also

### Managing path contents

var isEmpty: Bool

A Boolean that indicates whether this path is empty.

var count: Int

The number of elements in this path.

func removeLast(Int)

Removes values from the end of this path.

