

- Endpoint Security
-  es_event_lw_session_lock_t 

Structure

# es_event_lw_session_lock_t

Mac CatalystmacOS

``` source
struct es_event_lw_session_lock_t
```

## Topics

### Initializers

init()

init(username: es_string_token_t, graphical_session_id: es_graphical_session_id_t)

### Instance Properties

var graphical_session_id: es_graphical_session_id_t

var username: es_string_token_t

## Relationships

### Conforms To

- BitwiseCopyable

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

struct es_event_lw_session_login_t

