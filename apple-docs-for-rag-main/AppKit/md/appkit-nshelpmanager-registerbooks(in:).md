

- AppKit
- NSHelpManager
-  registerBooks(in:) 

Instance Method

# registerBooks(in:)

Registers one or more help books in the given bundle.

macOS 10.6+

``` source
@MainActor
func registerBooks(in bundle: Bundle) -> Bool
```

## Parameters 

`bundle`  

The bundle for additional help books. Books in the main bundle are automatically registered.

## Return Value

true if registration is successful, false if the bundle doesn’t contain any help books or if registration fails.

## Discussion

You use `registerBooksInBundle:` to register help books in, for example, a plug-in bundle. The `Info.plist` in the bundle should contain a help book directory path, which specifies one or more folders containing help books.

The main bundle is automatically registered by openHelpAnchor(_:inBook:) and find(_:inBook:).

