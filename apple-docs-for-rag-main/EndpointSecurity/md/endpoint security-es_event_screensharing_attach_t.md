

- Endpoint Security
-  es_event_screensharing_attach_t 

Structure

# es_event_screensharing_attach_t

Mac CatalystmacOS

``` source
struct es_event_screensharing_attach_t
```

## Topics

### Initializers

init()

init(success: Bool, source_address_type: es_address_type_t, source_address: es_string_token_t, viewer_appleid: es_string_token_t, authentication_type: es_string_token_t, authentication_username: es_string_token_t, session_username: es_string_token_t, existing_session: Bool, graphical_session_id: es_graphical_session_id_t)

### Instance Properties

var authentication_type: es_string_token_t

var authentication_username: es_string_token_t

var existing_session: Bool

var graphical_session_id: es_graphical_session_id_t

var session_username: es_string_token_t

var source_address: es_string_token_t

var source_address_type: es_address_type_t

var success: Bool

var viewer_appleid: es_string_token_t

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

struct es_event_lw_session_lock_t

