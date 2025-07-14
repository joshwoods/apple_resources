

- ContactProvider
- ContactItemEnumerator
-  invalidate() 

Instance Method

# invalidate()

Invalidates the enumerator.

iOS 18.0+iPadOS 18.0+

``` source
func invalidate() async
```

**Required**

## Discussion

The system calls this method before terminating the extension. The extension may terminate before this method returns.

