

- Endpoint Security
- es_process_t
-  parent_audit_token 

Instance Property

# parent_audit_token

The audit token of the parent process.

Mac CatalystmacOS

``` source
var parent_audit_token: audit_token_t
```

## Discussion

This field is only available if the message version is `4` or greater.

## See Also

### Inspecting Audit Tokens

var responsible_audit_token: audit_token_t

The audit token of the process responsible for this process.

