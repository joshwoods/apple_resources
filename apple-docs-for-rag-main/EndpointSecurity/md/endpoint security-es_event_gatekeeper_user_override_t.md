

- Endpoint Security
-  es_event_gatekeeper_user_override_t 

Structure

# es_event_gatekeeper_user_override_t

Mac CatalystmacOS

``` source
struct es_event_gatekeeper_user_override_t
```

## Topics

### Initializers

init()

init(file_type: es_gatekeeper_user_override_file_type_t, file: es_event_gatekeeper_user_override_t.__Unnamed_union_file, sha256: UnsafeMutablePointer&lt;es_sha256_t>?, signing_info: UnsafeMutablePointer&lt;es_signed_file_info_t>?)

### Instance Properties

var file: es_event_gatekeeper_user_override_t.__Unnamed_union_file

var file_type: es_gatekeeper_user_override_file_type_t

var sha256: UnsafeMutablePointer&lt;es_sha256_t>?

var signing_info: UnsafeMutablePointer&lt;es_signed_file_info_t>?

## See Also

### Structures

struct es_authorization_result_t

struct es_btm_launch_item_t

struct es_event_authentication_auto_unlock_t

struct es_event_authentication_od_t

struct es_event_authentication_t

struct es_event_authentication_token_t

struct es_event_authentication_touchid_t

struct es_event_authorization_judgement_t

struct es_event_authorization_petition_t

struct es_event_btm_launch_item_add_t

struct es_event_btm_launch_item_remove_t

struct es_event_login_login_t

struct es_event_login_logout_t

struct es_event_lw_session_lock_t

struct es_event_lw_session_login_t

