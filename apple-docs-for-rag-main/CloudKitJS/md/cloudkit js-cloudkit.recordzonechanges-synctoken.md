

- CloudKit JS
- CloudKit.RecordZoneChanges
-  syncToken 

Instance Property

# syncToken

Identifies a point in the zone’s change history. The first time you get record changes, omit this key and if `moreComing` is `true` in the response, use the `syncToken` in the response in the next request until `moreComing` is `false`. Otherwise, get the current sync token by fetching a zone.

CloudKit JS 1.0+

``` source
attribute String syncToken;
```

