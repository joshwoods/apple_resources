

- Safari Services
- SFSafariViewController
-  init(url:configuration:) 

Initializer

# init(url:configuration:)

Initializes and configures a Safari view controller that loads the specified URL.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    url URL: URL,
    configuration: SFSafariViewController.Configuration
)
```

## Parameters 

`URL`  

The URL to navigate to. The URL must use the `http` or `https` scheme.

`configuration`  

The configuration for the new view controller.

## Return Value

A newly created Safari view controller.

## Discussion

Use init(url:) to initialize an instance with the default configuration. The initializer copies the specified SFSafariViewController.Configuration object, so mutating the configuration after invoking the initializer has no effect on the view controller.

## See Also

### Creating a View Controller

class Configuration

A configuration object that defines how a Safari view controller should be initialized.

convenience init(url: URL)

Initializes a Safari view controller that loads the specified URL.

init(url: URL, entersReaderIfAvailable: Bool)

Initializes a Safari view controller that will load the specified URL, entering Reader mode if Reader mode is requested and available.

Deprecated

