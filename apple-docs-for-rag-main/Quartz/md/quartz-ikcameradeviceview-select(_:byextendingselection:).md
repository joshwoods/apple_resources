

- Quartz
- IKCameraDeviceView
-  select(\_:byExtendingSelection:) 

Instance Method

# select(\_:byExtendingSelection:)

Invoked to select the specified files, extending the selection if specified.

macOS 10.6+

``` source
@MainActor
func select(
    _ indexes: IndexSet!,
    byExtendingSelection extend: Bool
)
```

## Parameters 

`indexes`  

The indexes of the files to select.

`extend`  

true if the selection should be extended, otherwise false.

## See Also

### Selection Management

func selectedIndexes() -> IndexSet!

The selected indexes of the camera files.

