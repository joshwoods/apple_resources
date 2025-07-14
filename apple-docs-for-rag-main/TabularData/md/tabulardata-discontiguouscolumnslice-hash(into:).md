

- TabularData
- DiscontiguousColumnSlice
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the column slice by feeding them into a hasher.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func hash(into hasher: inout Hasher)
```

Available when `WrappedElement` conforms to `Hashable`.

## Parameters 

`hasher`  

A hasher the method uses to combine the components of the column slice.

