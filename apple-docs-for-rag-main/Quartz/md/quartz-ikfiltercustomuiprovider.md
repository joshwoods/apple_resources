

- Quartz
-  IKFilterCustomUIProvider 

Protocol

# IKFilterCustomUIProvider

A protocol used to provide a custom UI.

macOS 10.4+

``` source
protocol IKFilterCustomUIProvider
```

## Overview

The `IKFilterCustomUIProvider` protocol is an addition to the CIFilter class that defines a method for providing a view for a filter. This protocol is implemented by any filter that provides its own user interface.

## Topics

### Providing a Custom View

func provideView(forUIConfiguration: [AnyHashable : Any]!, excludedKeys: [Any]!) -> IKFilterUIView!

Provides a custom view for a filter.

**Required**

## See Also

### Protocols

protocol IKCameraDeviceViewDelegate

The `IKCameraDeviceViewDelegate` protocol is adopted by the delegate of the IKCameraDeviceView class. It allows downloading of camera content, handling selection changes, and handling errors.

protocol IKDeviceBrowserViewDelegate

The `IKDeviceBrowserViewDelegate` defines the methods that the delegate of the IKDeviceBrowserView class can implement. All the methods are optional.

IKImageBrowserDataSource Protocol

The `IKImageBrowserDataSource` informal protocol declares the methods that an instance of the IKImageBrowserView class uses to access the contents of its data source object.

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

