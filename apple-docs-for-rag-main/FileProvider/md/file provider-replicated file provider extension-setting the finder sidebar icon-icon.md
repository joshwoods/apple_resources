

- File Provider
- Replicated File Provider extension
-  Setting the Finder Sidebar Icon 

Article

# Setting the Finder Sidebar Icon

Specify a standard or custom symbol as a sidebar icon.

## Overview

To set the sidebar icon for your File Provider extension, set the CFBundleSymbolName key in the File Provider extension’s `Info.plist` file. The key takes the name of one of the SF Symbols. For the complete list of available symbols, see SF Symbols 3.

This image shows setting the sidebar icon to the `cloud.bolt.fill` symbol in the Plist editor.

Alternatively, you can open the `Info.plist` file as source code and edit the XML directly.

```
```

To create a custom symbol for your app, see Creating custom symbol images for your app. To see a sample code project that uses a custom symbol, see Synchronizing files using file provider extensions.

## See Also

### Essentials

Synchronizing the File Provider Extension

Keep the local and remote copies of your File Provider extension’s content in sync.

Synchronizing files using file provider extensions

Make remote files available in macOS and iOS, and synchronize their states by using file provider extensions.

