

- File Provider
- NSFileProviderItemProtocol
-  symlinkTargetPath 

Instance Property

# symlinkTargetPath

The target of the symlink.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
optional var symlinkTargetPath: String? { get }
```

## Discussion

If the extension contains an item with a typeIdentifier of `public.symlink` (`kUTTypeSymLink`), this property contains the symlink’s target. Otherwise, it’s `nil`.

## See Also

### Specifying Content Location

var parentItemIdentifier: NSFileProviderItemIdentifier

The persistent identifier of the item’s parent folder.

**Required**

var isTrashed: Bool

A Boolean value that indicates whether an item is in the trash.

