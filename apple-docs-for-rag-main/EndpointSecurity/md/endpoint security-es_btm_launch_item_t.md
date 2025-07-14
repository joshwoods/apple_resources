

- Endpoint Security
-  es_btm_launch_item_t 

Structure

# es_btm_launch_item_t

Mac CatalystmacOS

``` source
struct es_btm_launch_item_t
```

## Topics

### Initializers

init()

init(item_type: es_btm_item_type_t, legacy: Bool, managed: Bool, uid: uid_t, item_url: es_string_token_t, app_url: es_string_token_t)

### Instance Properties

var app_url: es_string_token_t

var item_type: es_btm_item_type_t

var item_url: es_string_token_t

var legacy: Bool

var managed: Bool

var uid: uid_t

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct es_authorization_result_t

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

struct es_event_lw_session_login_t

