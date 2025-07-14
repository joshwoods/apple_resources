

- CloudKit JS
- CloudKit.Container
-  acceptShares 

Instance Method

# acceptShares

Accepts a share—that is represented by a `shortGUID`—on behalf of the current user.

CloudKit JS 1.0+

``` source
Promise acceptShares(
 String[] shortGUIDs
);
```

## Parameters 

`shortGUIDs`  

One or more short GUIDs that represent shared records.

## Return Value

A `Promise` object that resolves to a CloudKit.RecordInfosResponse object, or rejects to a CKError object.

## See Also

### Accepting Shared Records

fetchRecordInfos

Returns information about a record for which you have a `shortGUID` property.

