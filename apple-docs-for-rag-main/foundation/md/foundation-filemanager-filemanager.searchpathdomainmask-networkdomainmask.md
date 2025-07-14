

- Foundation
- FileManager
- FileManager.SearchPathDomainMask
-  networkDomainMask 

Type Property

# networkDomainMask

The place to install items available on the network (`/Network`).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var networkDomainMask: FileManager.SearchPathDomainMask { get }
```

## See Also

### Specifying Search Path Domains

static var userDomainMask: FileManager.SearchPathDomainMask

The user’s home directory—the place to install user’s personal items (`~`).

static var localDomainMask: FileManager.SearchPathDomainMask

The place to install items available to everyone on this machine.

static var systemDomainMask: FileManager.SearchPathDomainMask

A directory for system files provided by Apple (`/System`) .

static var allDomainsMask: FileManager.SearchPathDomainMask

All domains.

