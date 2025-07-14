

- Quartz
- IKImageEditPanel
-  dataSource 

Instance Property

# dataSource

Specifies the edit panel’s dataSource.

macOS 10.5+

``` source
@MainActor
unowned(unsafe) var dataSource: (any IKImageEditPanelDataSource)! { get set }
```

## See Also

### Getting, Setting, and Reloading Data

func reloadData()

Reloads the data from the data associated with an image editing panel.

