

- Endpoint Security
-  es_tcc_event_type_t 

Structure

# es_tcc_event_type_t

Mac CatalystmacOS

``` source
struct es_tcc_event_type_t
```

## Overview

Represent the type of TCC modification event.

- ES_TCC_EVENT_TYPE_UNKNOWN: Unknown prior state.

- ES_TCC_EVENT_TYPE_CREATE: A new TCC authorization record was created.

- ES_TCC_EVENT_TYPE_MODIFY: An existing TCC authorization record was modified.

- ES_TCC_EVENT_TYPE_DELETE: An existing TCC authorization record was deleted.

## Topics

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

