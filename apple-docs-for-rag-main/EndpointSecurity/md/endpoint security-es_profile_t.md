

- Endpoint Security
-  es_profile_t 

Structure

# es_profile_t

Mac CatalystmacOS

``` source
struct es_profile_t
```

## Topics

### Initializers

init()

init(identifier: es_string_token_t, uuid: es_string_token_t, install_source: es_profile_source_t, organization: es_string_token_t, display_name: es_string_token_t, scope: es_string_token_t)

### Instance Properties

var display_name: es_string_token_t

var identifier: es_string_token_t

var install_source: es_profile_source_t

var organization: es_string_token_t

var scope: es_string_token_t

var uuid: es_string_token_t

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

