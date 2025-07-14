

- ContactProvider
-  ContactProviderExtension 

Protocol

# ContactProviderExtension

The protocol your app extension implements, which provides contact items to the system-wide Contacts ecosystem.

iOS 18.0+iPadOS 18.0+

``` source
protocol ContactProviderExtension : ContactItemEnumerating, AppExtension
```

## Overview

For the system to recognize your app extension, use the following identifier in the extension’s `Info.plist` file:

```
EXAppExtensionAttributes

    EXExtensionPointIdentifier
    com.apple.contact.provider.extension

```

Installing the host app installs your extension, but the system won’t run the extension until the extension domain is enabled. When the extension runs, the system first calls the extension’s configure(for:) method. Then you set up the enumerator that provides contact items from your data store.

The following shows a basic implementation of a `ContactProviderExtension`. Because `ContactProviderExtension` inherits from ContactItemEnumerating the implementation also implements enumerator(for:) which returns a ContactItemEnumerator on demand. In this example, the extension sets up a `RootContainerEnumerator` to provide its contact items; see the ContactItemEnumerator discussion for details of how `RootContainerEnumerator` works.

```
import ContactProvider

@main
class ExtensionExample: ContactProviderExtension {
    private let rootContainerEnumerator: RootContainerEnumerator

    required init() {
        rootContainerEnumerator = RootContainerEnumerator()
    }

    func configure(for domain: ContactProviderDomain) {
        rootContainerEnumerator.configure(for: domain)
    }

    func enumerator(for collection: ContactItem.Identifier) -> any ContactItemEnumerator {
        return rootContainerEnumerator
    }

    func invalidate() async {
        // Stop the enumeration and clean up, in preparation for the extension to terminate.
    }
}
```

## Topics

### Configuring an extension

func configure(for: any ContactProviderDomain)

Configures the extension instance for a domain.

**Required**

### Managing the extension life cycle

func invalidate() async throws

Invalidates the extension.

**Required**

## Relationships

### Inherits From

- AppExtension
- ContactItemEnumerating

