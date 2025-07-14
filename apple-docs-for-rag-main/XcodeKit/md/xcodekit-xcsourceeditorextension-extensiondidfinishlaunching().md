

- XcodeKit
- XCSourceEditorExtension
-  extensionDidFinishLaunching() 

Instance Method

# extensionDidFinishLaunching()

Tells the extension that it successfully launched and may begin to receive editor commands.

macOS 10.12+

``` source
optional func extensionDidFinishLaunching()
```

## Discussion

There are no guarantees about the thread or queue on which this method is called.

