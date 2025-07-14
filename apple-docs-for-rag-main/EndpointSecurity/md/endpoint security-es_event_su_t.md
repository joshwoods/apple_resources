

- Endpoint Security
-  es_event_su_t 

Structure

# es_event_su_t

Mac CatalystmacOS

``` source
struct es_event_su_t
```

## Topics

### Initializers

init()

init(success: Bool, failure_message: es_string_token_t, from_uid: uid_t, from_username: es_string_token_t, has_to_uid: Bool, to_uid: es_event_su_t.__Unnamed_union_to_uid, to_username: es_string_token_t, shell: es_string_token_t, argc: Int, argv: UnsafeMutablePointer&lt;es_string_token_t>?, env_count: Int, env: UnsafeMutablePointer&lt;es_string_token_t>?)

### Instance Properties

var argc: Int

var argv: UnsafeMutablePointer&lt;es_string_token_t>?

var env: UnsafeMutablePointer&lt;es_string_token_t>?

var env_count: Int

var failure_message: es_string_token_t

var from_uid: uid_t

var from_username: es_string_token_t

var has_to_uid: Bool

var shell: es_string_token_t

var success: Bool

var to_uid: es_event_su_t.__Unnamed_union_to_uid

var to_username: es_string_token_t

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

