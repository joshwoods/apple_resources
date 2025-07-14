

- Endpoint Security
-  es_event_openssh_login_t 

Structure

# es_event_openssh_login_t

Mac CatalystmacOS

``` source
struct es_event_openssh_login_t
```

## Topics

### Initializers

init()

init(success: Bool, result_type: es_openssh_login_result_type_t, source_address_type: es_address_type_t, source_address: es_string_token_t, username: es_string_token_t, has_uid: Bool, uid: es_event_openssh_login_t.__Unnamed_union_uid)

### Instance Properties

var has_uid: Bool

var result_type: es_openssh_login_result_type_t

var source_address: es_string_token_t

var source_address_type: es_address_type_t

var success: Bool

var uid: es_event_openssh_login_t.__Unnamed_union_uid

var username: es_string_token_t

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

struct es_event_gatekeeper_user_override_t

struct es_event_login_login_t

struct es_event_login_logout_t

struct es_event_lw_session_lock_t

