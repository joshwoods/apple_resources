

- ContactProvider
- ContactProviderExtension
-  invalidate() 

Instance Method

# invalidate()

Invalidates the extension.

iOS 18.0+iPadOS 18.0+

``` source
func invalidate() async throws
```

**Required**

## Discussion

The system calls this method before terminating the extension. The extension may complete termination before this method returns.

