

- iAd
- ADClient
-  shared() Deprecated

Type Method

# shared()

Gets an instance of ADClient.

``` source
class func shared() -> ADClient
```

Deprecated

This has been replaced by functionality in AdServices.framework's AAAttribution class.

## Return Value

An instance of ADClient.

## Discussion

Use the `ADClient` instance to obtain attribution details.

Note

This method no longer returns a singleton. This change results in a small savings in memory usage by freeing up objects that aren’t required after the request for attribution details completes.

```
ADClient.shared.requestAttributionDetails()
```

```
```

