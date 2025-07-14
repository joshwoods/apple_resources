

- Endpoint Security
- es_event_authorization_petition_t
-  init(instigator:petitioner:flags:right_count:rights:instigator_token:petitioner_token:) 

Initializer

# init(instigator:petitioner:flags:right_count:rights:instigator_token:petitioner_token:)

Mac CatalystmacOS

``` source
init(
    instigator: UnsafeMutablePointer?,
    petitioner: UnsafeMutablePointer?,
    flags: UInt32,
    right_count: Int,
    rights: UnsafeMutablePointer?,
    instigator_token: audit_token_t,
    petitioner_token: audit_token_t
)
```

