

- Assets Library
- ALAssetsGroup
-  add(\_:) Deprecated

Instance Method

# add(\_:)

Adds an existing asset to the receiver.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func add(_ asset: ALAsset!) -> Bool
```

Deprecated

Use addAssets: on a PHAssetCollectionChangeRequest: created from a PHAssetCollection in the Photos framework instead

## Parameters 

`asset`  

The asset to add to the receiver.

## Return Value

true if `asset` was added successfully, otherwise false.

## Discussion

The method may fail (return false) if the group is not editable, or if the asset could not be added to the group.

You should check the isEditable property of the group to see if it is possible to add an asset to the group.

## See Also

### Adding Assets

var isEditable: Bool

Indicates whether the application can edit the group.

Deprecated

