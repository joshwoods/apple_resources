

- os
- Logging
-  Customizing Logging Behavior While Debugging 

Article

# Customizing Logging Behavior While Debugging

Control which log events are recorded.

## Overview

Logging behavior is normally governed by the system. However, while debugging in macOS, you can enable different logging levels for a subsystem using the `log` command-line tool’s `config` argument while logged in as root. The example below shows how to enable debug-level logging for a subsystem:

```
```

Use the `log` tool’s `status` argument to check the current logging level of a subsystem:

```
```

You can also override the logging behavior of a specific subsystem by creating and installing a logging configuration profile property list file in the `/Library/Preferences/Logging/Subsystems/` directory. Name the file using an identifier string, in reverse DNS notation that identifies, for example, `com.your_company.your_subsystem_name.plist`. Next, add one or more settings dictionaries to the top level of the file. A `DEFAULT-OPTIONS` settings dictionary defines global behavior settings for the entire subsystem. Category settings dictionaries define behavior for specific categories of messages within the subsystem. The example below shows the top-level structure of a logging configuration profile:

```
```

Each settings dictionary within a logging profile contains a `Level` subdictionary, which contains the following setting keys:

| Key | Description |
|----|----|
| `Enable` | Enables a specific log level. |
| `Persist` | Controls whether messages are stored in memory and then saved to the data store, or stored in memory only. |

The `Enable` key and `Persist` key both accept the following string values:

| Value | Description |
|----|----|
| `Inherit` | Explicitly states that the subsystem or category inherits the behavior of its parent. In the case of a category, the parent is the subsystem. In the case of a subsystem, the parent is the system. |
| `Default` | Only default-level messages are captured. |
| `Info` | Default-level and info-level messages are captured. |
| `Debug` | Default-level, info-level, and debug-level messages are captured. |

The example below shows a `Level` subdictionary that enables info-level logging that inherits the persistence behavior of a subsystem or the system:

```
```

The example below shows a complete logging profile, which configures a subsystem to perform info-level logging and a `server-connections` category within the subsystem to perform debug-level logging:

```
```

Note

Subsystems inherit the logging behavior of the system, and categories inherit the behavior of the subsystem in which they reside. Therefore, settings only need to be specified if they differ from the inherited behavior.

## See Also

### Essentials

Generating Log Messages from Your Code

Record useful debugging and analysis information, and include dynamic content in your messages.

Viewing Log Messages

Use various tools to retrieve log information.

