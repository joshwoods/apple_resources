

- Foundation
- URL
-  deletingLastPathComponent() 

Instance Method

# deletingLastPathComponent()

Returns a URL constructed by removing the last path component of self.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deletingLastPathComponent() -> URL
```

## Discussion

This function may either remove a path component or append `/..`.

If the URL has an empty path (e.g., `http://www.example.com`), then this function will return the URL unchanged.

## See Also

### Removing path components

func deleteLastPathComponent()

Returns a URL constructed by removing the last path component of self.

