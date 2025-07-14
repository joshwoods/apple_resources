

- Assets Library
- ALAssetsGroup
-  isEditable Deprecated

Instance Property

# isEditable

Indicates whether the application can edit the group.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isEditable: Bool { get }
```

Deprecated

Use canPerformEditOperation: on a PHAssetCollection from the Photos framework instead

## Discussion

The value of the property is true if the application is able to edit the group, otherwise it is false.

## See Also

### Adding Assets

func add(ALAsset!) -> Bool

Adds an existing asset to the receiver.

Deprecated

