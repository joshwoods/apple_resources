

- CKTool JS
- CKDBResolvedRecord
-  webpageUrl 

Instance Property

# webpageUrl

The fallback URL that you can redirect users to if the operation fails.

CKTool JS 1.2.15+

``` source
attribute string? webpageUrl;
```

## Discussion

An operation might fail, if a resolve/accept endpoint doesn’t succeed. If that happens, this value would be the URL that you could redirect users to. You can set the fallback URL using CloudKit Dashboard.

