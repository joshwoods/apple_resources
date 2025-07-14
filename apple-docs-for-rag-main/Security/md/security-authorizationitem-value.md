

- Security
- AuthorizationItem
-  value 

Instance Property

# value

A pointer to information pertaining to the name field.

Mac Catalyst 13.0+macOS 10.0+

``` source
var value: UnsafeMutableRawPointer?
```

## Discussion

If the `name` field is set to the value represented by the constant kAuthorizationRightExecute, then set the `value` field to the full POSIX pathname of the tool you want to execute. In most other cases, set this field to `NULL`.

