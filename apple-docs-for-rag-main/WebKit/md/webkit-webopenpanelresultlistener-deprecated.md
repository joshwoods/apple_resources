

- WebKit
-  WebOpenPanelResultListener Deprecated

Protocol

# WebOpenPanelResultListener

`WebView` user interface delegates that implement the webView:runOpenPanelForFileButtonWithResultListener: method use the methods defined in this protocol to communicate with the listener object. The methods allow the delegate to send a cancel message, or set the selected file name.

macOS 10.3–10.14Deprecated

``` source
protocol WebOpenPanelResultListener : NSObjectProtocol
```

## Topics

### Setting a File Name

func chooseFilename(String!)

Displays a file open panel and returns the selected filename.

**Required**

func chooseFilenames([Any]!)

Displays a file open panel and returns the multiple selected filenames.

**Required**

### Cancelling a File Open Operation

func cancel()

Invoked when a file open operation was cancelled.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

