

- CloudKit JS
- CloudKit.Response
-  errors 

Instance Property

# errors

Errors that occurred in the request.

CloudKit JS 1.0+

``` source
readonly attribute CloudKit.CKError[] errors;
```

## Discussion

There’s one CKError object for each individual operation that failed.

## See Also

### Handling Errors

hasErrors

A Boolean value indicating whether errors occurred in the request.

