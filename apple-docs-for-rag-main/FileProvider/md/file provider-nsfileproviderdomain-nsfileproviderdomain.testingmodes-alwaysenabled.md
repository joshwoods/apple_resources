

- File Provider
- NSFileProviderDomain
- NSFileProviderDomain.TestingModes
-  alwaysEnabled 

Type Property

# alwaysEnabled

A testing mode that automatically enables the domain.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
static var alwaysEnabled: NSFileProviderDomain.TestingModes { get }
```

## Discussion

By default, the user must manually enable a domain in System Preferences \> Extensions before the File Provider extension can access it. This testing mode bypasses that workflow and automatically enables the domain.

## See Also

### Accessing Modes

static var interactive: NSFileProviderDomain.TestingModes

A testing mode where the extension can deterministically test asynchronous operations.

