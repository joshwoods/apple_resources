

- Quartz
- IKScannerDeviceViewDelegate
-  scannerDeviceView(\_:didScanTo:fileData:error:) 

Instance Method

# scannerDeviceView(\_:didScanTo:fileData:error:)

Invoked when the scan has completed and the data is available.

macOS 10.10+

``` source
optional func scannerDeviceView(
    _ scannerDeviceView: IKScannerDeviceView!,
    didScanTo url: URL!,
    fileData data: Data!,
    error: (any Error)!
)
```

## Parameters 

`scannerDeviceView`  

The scanner device that sent the message.

`url`  

The URL to save the data.

`data`  

The data from the scan.

`error`  

Any error encountered during the scan.

## Discussion

This method is called when the scan has completed..

If the `scannerDeviceView` transferMode is IKScannerDeviceViewTransferMode.fileBased, the scan will have been saved at the specified `url`. The URL will be in the download directory and be a complete path, including a ‘sequence number’ if the file already exists.

If the `scannerDeviceView` transferMode is IKScannerDeviceViewTransferMode.memoryBased, the scanned data is contained in the data parameter. You can then take the action appropriate to your application.

In case of an error, the parameters (`url` and `data`) will be `NULL` and `error` (which may come directly from the scanner module / or the ImageCaptureCore framework) will describe why the scan or save failed.

