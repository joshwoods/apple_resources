

- CKTool JS
- Configuration
-  jsonStringify 

Instance Property

# jsonStringify

A function that a request function uses to prepare JSON to send to the API server.

CKTool JS 1.2.15+

``` source
attribute Function jsonStringify;
```

## Discussion

The API server can receive numbers larger than the default JavaScript JSON stringify function can handle, so this function is expected to handle large numbers.

This value is only set when `Configuration` is constructed.

