

- Safari Services
- SFSafariViewController
-  init(url:) 

Initializer

# init(url:)

Initializes a Safari view controller that loads the specified URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(url URL: URL)
```

## Parameters 

`URL`  

The URL to navigate to. The URL must use the `http` or `https` scheme.

## Return Value

A newly created Safari view controller.

## See Also

### Creating a View Controller

init(url: URL, configuration: SFSafariViewController.Configuration)

Initializes and configures a Safari view controller that loads the specified URL.

class Configuration

A configuration object that defines how a Safari view controller should be initialized.

init(url: URL, entersReaderIfAvailable: Bool)

Initializes a Safari view controller that will load the specified URL, entering Reader mode if Reader mode is requested and available.

Deprecated

