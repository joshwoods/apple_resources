

- Foundation
- FileManager
- FileManager.SearchPathDomainMask
-  localDomainMask 

Type Property

# localDomainMask

The place to install items available to everyone on this machine.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var localDomainMask: FileManager.SearchPathDomainMask { get }
```

## See Also

### Specifying Search Path Domains

static var userDomainMask: FileManager.SearchPathDomainMask

The user’s home directory—the place to install user’s personal items (`~`).

static var networkDomainMask: FileManager.SearchPathDomainMask

The place to install items available on the network (`/Network`).

static var systemDomainMask: FileManager.SearchPathDomainMask

A directory for system files provided by Apple (`/System`) .

static var allDomainsMask: FileManager.SearchPathDomainMask

All domains.

