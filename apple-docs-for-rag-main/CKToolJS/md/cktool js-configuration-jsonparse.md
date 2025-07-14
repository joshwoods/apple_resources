

- CKTool JS
- Configuration
-  jsonParse 

Instance Property

# jsonParse

A function that a response parser uses to interpret JSON from the API server.

CKTool JS 1.2.15+

``` source
attribute Function jsonParse;
```

## Discussion

The API server can send numbers larger than the default JavaScript JSON parse function can handle, so this function is expected to handle large numbers.

This value is only set when `Configuration` is constructed.

