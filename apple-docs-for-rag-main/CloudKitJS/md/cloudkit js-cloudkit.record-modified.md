

- CloudKit JS
- CloudKit.Record
-  modified 

Instance Property

# modified

Information about when the record was last modified. The properties of this object are: `timestamp` (`Number`), the time at which the record was created, and `user` (`String`), the ID of the user who modified the record. This field is used by the CloudKit.RecordsResponse class. This value of this field is set by the server. Omit this key when saving a record.

CloudKit JS 1.0+

``` source
attribute Object modified;
```

