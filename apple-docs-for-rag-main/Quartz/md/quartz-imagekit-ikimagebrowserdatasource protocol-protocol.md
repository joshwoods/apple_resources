

- Quartz
- ImageKit
-  IKImageBrowserDataSource Protocol 

# IKImageBrowserDataSource Protocol

The `IKImageBrowserDataSource` informal protocol declares the methods that an instance of the IKImageBrowserView class uses to access the contents of its data source object.

## Topics

### Providing Information About Items (Required)

func numberOfItems(inImageBrowser aBrowser: IKImageBrowserView!) -> Int

Returns the number of records managed by the data source object.

func imageBrowser(_ aBrowser: IKImageBrowserView!, itemAt index: Int) -> Any!

Returns an object for the item in an image browser view that corresponds to the specified index.

### Supporting Item Editing (Optional)

func imageBrowser(_ aBrowser: IKImageBrowserView!, removeItemsAt indexes: IndexSet!)

Signals that a remove operation should be applied to the specified items.

func imageBrowser(_ aBrowser: IKImageBrowserView!, moveItemsAt indexes: IndexSet!, to destinationIndex: Int) -> Bool

Signals that the specified items should be moved to the specified destination.

func imageBrowser(_ aBrowser: IKImageBrowserView!, writeItemsAt itemIndexes: IndexSet!, to pasteboard: NSPasteboard!) -> Int

Signals that a drag should begin.

### Providing Information About Groups (Optional)

func numberOfGroups(inImageBrowser aBrowser: IKImageBrowserView!) -> Int

Returns the number of groups in an image browser view.

func imageBrowser(_ aBrowser: IKImageBrowserView!, groupAt index: Int) -> [AnyHashable : Any]!

Returns the group at the specified index.

## See Also

### Protocols

protocol IKCameraDeviceViewDelegate

The `IKCameraDeviceViewDelegate` protocol is adopted by the delegate of the IKCameraDeviceView class. It allows downloading of camera content, handling selection changes, and handling errors.

protocol IKDeviceBrowserViewDelegate

The `IKDeviceBrowserViewDelegate` defines the methods that the delegate of the IKDeviceBrowserView class can implement. All the methods are optional.

protocol IKFilterCustomUIProvider

A protocol used to provide a custom UI.

IKImageBrowserDelegate Protocol

The `IKImageBrowserDelegate` is an informal protocol for the delegate of an IKImageBrowserView object. You can implement these methods to perform custom tasks when in response to events in the image browser view.

IKImageBrowserItem Protocol

The `IKImageBrowserItem` informal protocol declares the methods that an instance of the IKImageBrowserView class uses to access the contents of its data source for a given item. Some of the methods in this protocol are needed frequently, so you should implement them efficiently.

protocol IKImageEditPanelDataSource

The `IKImageEditPanelDataSource` protocol describes the methods that an IKImageEditPanel object uses to access the contents of its data source object.

protocol IKScannerDeviceViewDelegate

The `IKScannerDeviceViewDelegate` protocol defines the delegate protocol that the IKScannerDeviceView delegate must conform to.

protocol IKSlideshowDataSource

The `IKSlideshowDataSource` protocol describes the methods that an IKSlideshow object uses to access the contents of its data source object.

