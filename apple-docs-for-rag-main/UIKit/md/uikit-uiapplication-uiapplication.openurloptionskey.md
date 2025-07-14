

- UIKit
- UIApplication
-  UIApplication.OpenURLOptionsKey 

Structure

# UIApplication.OpenURLOptionsKey

Keys you use to access values in the options dictionary when opening a URL.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct OpenURLOptionsKey
```

## Overview

Use these keys to retrieve options in the application(_:open:options:) method of your app delegate.

## Topics

### Accessing open-URL options

static let sourceApplication: UIApplication.OpenURLOptionsKey

A key containing the bundle ID of the app that sent the open-URL request to your app.

static let annotation: UIApplication.OpenURLOptionsKey

A key containing the information passed to a document interaction controller object’s annotation property.

static let openInPlace: UIApplication.OpenURLOptionsKey

A key containing a flag that indicates whether a document must be copied before you use it.

static let eventAttribution: UIApplication.OpenURLOptionsKey

### Creating an open-URL options key

init(rawValue: String)

Creates a URL-opening options key with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Opening a URL-specified resource

func application(UIApplication, open: URL, options: [UIApplication.OpenURLOptionsKey : Any]) -> Bool

Asks the delegate to open a resource specified by a URL, and provides a dictionary of launch options.

