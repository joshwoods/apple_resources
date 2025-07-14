

- CloudKit JS
- CloudKit.Database
-  shareWithUI 

Instance Method

# shareWithUI

Presents a UI to the user which lets them share a record with other users.

CloudKit JS 1.0+

``` source
Promise shareWithUI(
 Object options
);
```

## Parameters 

`options`  

A dictionary containing options for the share UI:

| Key | Description |
|----|----|
| `record` | The CloudKit.Record object that is being shared. |
| `zoneID` | A CloudKit.ZoneID or zone name (`String`) that identifies the record zone in the database where you want to perform the operation. The default is the database default zone. This property is required. |
| `shareTitle` | The title (`String`) of the share. |
| `shareType` | The type (`String`) of the share. |
| `shareThumbnail` | A thumbnail (`String`) representing the share. |
| `supportedAccess` | The supported participant access to the share. An array of `String` objects with values `PRIVATE` or `PUBLIC`. |
| `supportedPermissions` | The supported read-write permissions for the share. An array of `String` objects with values `READ_WRITE` or `READ_ONLY`. |

## Return Value

A `Promise` object that resolves to an object that represents the share record, or rejects to a CKError object.

