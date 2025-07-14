

- Foundation
- URL
-  deletingPathExtension() 

Instance Method

# deletingPathExtension()

Returns a URL constructed by removing any path extension.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deletingPathExtension() -> URL
```

## Discussion

If the URL has an empty path (e.g., `http://www.example.com`), then this function will return the URL unchanged.

## See Also

### Removing a path extension

func deletePathExtension()

Returns a URL constructed by removing any path extension.

