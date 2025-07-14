

- File Provider
- NSFileProviderExtension
-  stopProvidingItem(at:) 

Instance Method

# stopProvidingItem(at:)

Tells the File Provider extension that a given document is no longer being accessed.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func stopProvidingItem(at url: URL)
```

## Parameters 

`url`  

The URL of a shared document.

## Discussion

The system calls this method as soon as all other processes have stopped accessing the given file. You can override this method to remove the document from the local file system, thus freeing up storage space. You must provide placeholders for any documents you remove.

You must override this method, even if you only provide an empty implementation. Do not call `super` in your implementations.

## See Also

### Managing shared files

func itemChanged(at: URL)

Tells the File Provider extension that a document has changed.

func providePlaceholder(at: URL, completionHandler: ((any Error)?) -> Void)

Triggers the creation of a placeholder for the given URL.

func startProvidingItem(at: URL, completionHandler: ((any Error)?) -> Void)

Provides an actual file on disk for a placeholder.

