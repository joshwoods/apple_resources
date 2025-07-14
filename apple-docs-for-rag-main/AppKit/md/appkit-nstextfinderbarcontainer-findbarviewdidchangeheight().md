

- AppKit
- NSTextFinderBarContainer
-  findBarViewDidChangeHeight() 

Instance Method

# findBarViewDidChangeHeight()

Notifies the find bar container that the find bar has changed its height.

macOS

``` source
func findBarViewDidChangeHeight()
```

**Required**

## Discussion

Upon receiving this message the container may be required to re-tile its contents.

