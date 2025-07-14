

- CloudKit JS
- CloudKit.Container
-  fetchRecordInfos 

Instance Method

# fetchRecordInfos

Returns information about a record for which you have a `shortGUID` property.

CloudKit JS 1.0+

``` source
Promise fetchRecordInfos(
 String[] shortGUIDs
);
```

## Parameters 

`shortGUIDs`  

One or more short GUIDs that represent records you want to fetch information about.

## Return Value

A `Promise` object that resolves to a CloudKit.RecordInfosResponse object, or rejects to a CKError object.

## Discussion

Use this method to show details about a record to a user before asking them to accept a share.

## See Also

### Accepting Shared Records

acceptShares

Accepts a share—that is represented by a `shortGUID`—on behalf of the current user.

