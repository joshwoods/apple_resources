

- Assets Library
- ALAssetsLibrary
-  enumerateGroupsWithTypes(\_:usingBlock:failureBlock:) Deprecated

Instance Method

# enumerateGroupsWithTypes(\_:usingBlock:failureBlock:)

iOS 9.0–9.0DeprecatediPadOS 9.0–9.0DeprecatedMac Catalyst 9.0–9.0Deprecated

``` source
@nonobjc
func enumerateGroupsWithTypes(
    _ types: UInt32,
    usingBlock enumerationBlock: ALAssetsLibraryGroupsEnumerationResultsBlock!,
    failureBlock: ALAssetsLibraryAccessFailureBlock!
)
```

## See Also

### Enumerating Assets

func enumerateGroups(withTypes: ALAssetsGroupType, using: ALAssetsLibraryGroupsEnumerationResultsBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Invokes a given block passing as a parameter each of the asset groups that match the given asset group type.

Deprecated

