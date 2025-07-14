

- Endpoint Security
- es_event_authorization_judgement_t
-  init(instigator:petitioner:return_code:result_count:results:instigator_token:petitioner_token:) 

Initializer

# init(instigator:petitioner:return_code:result_count:results:instigator_token:petitioner_token:)

Mac CatalystmacOS

``` source
init(
    instigator: UnsafeMutablePointer?,
    petitioner: UnsafeMutablePointer?,
    return_code: Int32,
    result_count: Int,
    results: UnsafeMutablePointer?,
    instigator_token: audit_token_t,
    petitioner_token: audit_token_t
)
```

