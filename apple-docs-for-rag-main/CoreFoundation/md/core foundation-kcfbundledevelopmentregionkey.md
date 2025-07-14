

- Core Foundation
-  kCFBundleDevelopmentRegionKey 

Global Variable

# kCFBundleDevelopmentRegionKey

The name of the development language of the bundle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFBundleDevelopmentRegionKey: CFString!
```

## Discussion

When CFBundle looks for resources, the fallback is to look in the lproj whose name is given by the `kCFBundleDevelopmentRegionKey` in the `Info.plist` file. You must, therefore, ensure that a bundle contains an lproj with that exact name containing a copy of every localized resource, otherwise CFBundle cannot guarantee the fallback mechanism will work.

## See Also

### Constants

let kCFBundleInfoDictionaryVersionKey: CFString!

The version of the information property list format.

let kCFBundleExecutableKey: CFString!

The name of the executable in this bundle (if any).

let kCFBundleIdentifierKey: CFString!

The bundle identifier.

let kCFBundleVersionKey: CFString!

The version number of the bundle.

let kCFBundleNameKey: CFString!

The human-readable name of the bundle.

let kCFBundleLocalizationsKey: CFString!

Allows an unbundled application that handles localization itself to specify which localizations it has available.

