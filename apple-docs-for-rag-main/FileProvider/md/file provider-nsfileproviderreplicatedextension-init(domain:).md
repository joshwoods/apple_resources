

- File Provider
- NSFileProviderReplicatedExtension
-  init(domain:) 

Initializer

# init(domain:)

Creates an instance of the file provider for the specified domain.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
init(domain: NSFileProviderDomain)
```

**Required**

## Parameters 

`domain`  

The domain for the file provider.

## See Also

### Creating and Removing File Providers

func invalidate()

Tells the file provider to perform any necessary cleanup so that the system can deallocate it.

**Required**

