

- CloudKit JS
- CloudKit.Record
-  created 

Instance Property

# created

Information about when the record was created on the server. The properties of this object are: `timestamp` (`Number`), the time at which the record was created, and `user` (`String`), the ID of the user who created the record. This field is used by the CloudKit.RecordsResponse class. The value of this field is set by the server. Omit this key when saving a record.

CloudKit JS 1.0+

``` source
attribute Object created;
```

