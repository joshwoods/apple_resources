

- Endpoint Security
-  ES_PROC_CHECK_TYPE_UDATA_INFO Deprecated

Global Variable

# ES_PROC_CHECK_TYPE_UDATA_INFO

A type of process check that involves a user data token.

Mac CatalystmacOS

``` source
var ES_PROC_CHECK_TYPE_UDATA_INFO: es_proc_check_type_t { get }
```

Deprecated

Endpoint Security no longer generates process check events with this type.

## Discussion

This type corresponds to the `proc_udata_info` function from libproc.h.

## See Also

### Constants

var ES_ADDRESS_TYPE_IPV4: es_address_type_t

var ES_ADDRESS_TYPE_IPV6: es_address_type_t

var ES_ADDRESS_TYPE_NAMED_SOCKET: es_address_type_t

var ES_ADDRESS_TYPE_NONE: es_address_type_t

var ES_AUTHENTICATION_TYPE_AUTO_UNLOCK: es_authentication_type_t

var ES_AUTHENTICATION_TYPE_LAST: es_authentication_type_t

var ES_AUTHENTICATION_TYPE_OD: es_authentication_type_t

var ES_AUTHENTICATION_TYPE_TOKEN: es_authentication_type_t

var ES_AUTHENTICATION_TYPE_TOUCHID: es_authentication_type_t

var ES_AUTHORIZATION_RULE_CLASS_ALLOW: es_authorization_rule_class_t

var ES_AUTHORIZATION_RULE_CLASS_DENY: es_authorization_rule_class_t

var ES_AUTHORIZATION_RULE_CLASS_INVALID: es_authorization_rule_class_t

var ES_AUTHORIZATION_RULE_CLASS_MECHANISM: es_authorization_rule_class_t

var ES_AUTHORIZATION_RULE_CLASS_RULE: es_authorization_rule_class_t

var ES_AUTHORIZATION_RULE_CLASS_UNKNOWN: es_authorization_rule_class_t

