

- Kernel
- Kernel Enumerations
-  mbuf_traffic_class_t 

Enumeration

# mbuf_traffic_class_t

Traffic class of a packet

macOS 10.7+

``` source
typedef enum mbuf_traffic_class_t : unsigned int {
    ...
} mbuf_traffic_class_t;
```

## Overview

Property that represent the category of traffic of a packet. This information may be used by the driver and at the link level.

## Topics

### Constants

MBUF_TC_BE

MBUF_TC_BK

MBUF_TC_VI

MBUF_TC_VO

