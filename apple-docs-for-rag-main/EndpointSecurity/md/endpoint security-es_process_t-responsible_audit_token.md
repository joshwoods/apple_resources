

- Endpoint Security
- es_process_t
-  responsible_audit_token 

Instance Property

# responsible_audit_token

The audit token of the process responsible for this process.

Mac CatalystmacOS

``` source
var responsible_audit_token: audit_token_t
```

## Discussion

The responsible process may be this process itself, if there’s no responsible process or the responsible process already exited.

This field is only available if the message version is `4` or greater.

## See Also

### Inspecting Audit Tokens

var parent_audit_token: audit_token_t

The audit token of the parent process.

