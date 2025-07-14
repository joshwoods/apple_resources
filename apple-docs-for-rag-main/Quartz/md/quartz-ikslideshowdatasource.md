

- Quartz
-  IKSlideshowDataSource 

Protocol

# IKSlideshowDataSource

The `IKSlideshowDataSource` protocol describes the methods that an IKSlideshow object uses to access the contents of its data source object.

macOS 10.4+

``` source
protocol IKSlideshowDataSource
```

## Overview

Important

Slide show data source methods may be called on secondary threads. When you implement these methods, you must ensure that they are safe to run on threads other than the main thread.

## Topics

### Providing Slideshow Information

func numberOfSlideshowItems() -> Int

Returns the number of items in a slideshow.

**Required**

func slideshowItem(at: Int) -> Any!

Returns the item for a given index

**Required**

func nameOfSlideshowItem(at: Int) -> String!

Returns the display name for item at the specified index.

func canExportSlideshowItem(at: Int, toApplication: String!) -> Bool

Reports whether the export button should be enabled for a slideshow item.

### Performing Custom Tasks

func slideshowWillStart()

Performs custom tasks when the slideshow is about to start.

func slideshowDidStop()

Performs custom tasks when the slideshow stops.

func slideshowDidChangeCurrentIndex(Int)

Performs custom tasks when the slideshow changes to the item at the specified index.

## See Also

### Protocols

protocol IKCameraDeviceViewDelegate

The `IKCameraDeviceViewDelegate` protocol is adopted by the delegate of the IKCameraDeviceView class. It allows downloading of camera content, handling selection changes, and handling errors.

protocol IKDeviceBrowserViewDelegate

The `IKDeviceBrowserViewDelegate` defines the methods that the delegate of the IKDeviceBrowserView class can implement. All the methods are optional.

protocol IKFilterCustomUIProvider

A protocol used to provide a custom UI.

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

