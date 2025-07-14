

- CloudKit JS
- CloudKit.Database
-  fetchDatabaseChanges 

Instance Method

# fetchDatabaseChanges

Fetch changed record zones in the database.

CloudKit JS 1.0+

``` source
Promise fetchDatabaseChanges(
 optional Object options
);
```

## Parameters 

`options`  

Options to fetch database changes. This `Dictionary` object has one key:

| Key | Description |
|----|----|
| `syncToken` | Identifies a point in the database’s change history. The first time you fetch changes, omit this key and if `moreComing` is `true` in the response, use the `syncToken` in the response in the next request until `moreComing` is `false`. |

## Return Value

A `Promise` object that resolves to a CloudKit.DatabaseChangesResponse object, or rejects to a CKError object.

## Discussion

For example, use this method to fetch the zones that changed and then use the fetchRecordZoneChanges method to fetch the changed records in each zone.

```
database.fetchDatabaseChanges().then(function(response) {
   return database.fetchRecordZoneChanges(response.zones)
})
.then(function(response) {
   response.zones.forEach(function(zone) {
       zone.records.forEach(function(record) {
          // Apply the record change
       })
   })
})
```

## See Also

### Fetching Changes

databaseScope

The type of database (public, private, or shared).

fetchRecordZoneChanges

Fetch changes to the specified record zones in the database.

