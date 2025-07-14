

- Safari Services
- SFSafariViewController
-  init(url:entersReaderIfAvailable:) Deprecated

Initializer

# init(url:entersReaderIfAvailable:)

Initializes a Safari view controller that will load the specified URL, entering Reader mode if Reader mode is requested and available.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init(
    url URL: URL,
    entersReaderIfAvailable: Bool
)
```

## Parameters 

`URL`  

The URL to navigate to. The URL must use the `http` or `https` scheme.

`entersReaderIfAvailable`  

On output, true if Reader mode should be entered automatically when it is available for the webpage; otherwise, false.

## Return Value

A newly created Safari view controller.

## Discussion

`entersReaderIfAvailable` applies only to the first page loaded.

## See Also

### Creating a View Controller

init(url: URL, configuration: SFSafariViewController.Configuration)

Initializes and configures a Safari view controller that loads the specified URL.

class Configuration

A configuration object that defines how a Safari view controller should be initialized.

convenience init(url: URL)

Initializes a Safari view controller that loads the specified URL.

