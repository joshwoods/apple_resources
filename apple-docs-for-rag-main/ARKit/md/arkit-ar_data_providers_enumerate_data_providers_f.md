

- ARKit
-  ar_data_providers_enumerate_data_providers_f 

Function

# ar_data_providers_enumerate_data_providers_f

Enumerates a collection of data providers.

visionOS 1.0+

``` source
extern void ar_data_providers_enumerate_data_providers_f(ar_data_providers_t data_providers, void * context, ar_data_providers_enumerator_function_t data_providers_enumerator_function);
```

## See Also

### Data providers

ar_data_provider_state_t

The possible states of a data provider.

ar_data_provider_get_required_authorization_type

The kinds of authorization you need to use a particular data provider type.

ar_data_provider_get_state

Gets the current status of data coming from this provider.

ar_data_providers_enumerator_t

A handler for enumerating a collection of data providers.

ar_data_providers_t

A collection of data providers.

ar_data_providers_add_data_provider

Adds a data provider to a collection.

ar_data_providers_add_data_providers

Adds multiple data providers to a collection.

ar_data_providers_create

Creates an empty collection of data providers.

ar_data_providers_create_with_data_providers

Creates a collection of data providers that contains the data providers you supply.

ar_data_providers_get_count

Gets the number of data providers in a collection.

ar_data_providers_enumerate_data_providers

Enumerates a collection of data providers.

ar_data_providers_remove_data_provider

Removes a data provider from a collection.

ar_data_providers_remove_data_providers

Removes multiple data providers from a collection.

ar_data_providers_enumerator_function_t

ar_session_data_provider_state_change_handler_function_t

