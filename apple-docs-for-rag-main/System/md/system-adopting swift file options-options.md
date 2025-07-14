

- System
-  Adopting Swift File Options 

Article

# Adopting Swift File Options

Migrate existing C code to Swift, using the file-operation options provided by the System module.

## Overview

The C options for how to open a file map to Swift as follows:

- `O_RDONLY` ⟶ readOnly

- `O_WRONLY` ⟶ writeOnly

- `O_RDWR` ⟶ readWrite

The C constants for specifying options when opening a file map to Swift as follows:

- `O_NONBLOCK` ⟶ nonBlocking

- `O_APPEND` ⟶ append

- `O_CREAT` ⟶ create

- `O_TRUNC` ⟶ truncate

- `O_EXCL` ⟶ exclusiveCreate

- `O_SHLOCK` ⟶ sharedLock

- `O_EXLOCK` ⟶ exclusiveLock

- `O_NOFOLLOW` ⟶ noFollow

- `O_SYMLINK` ⟶ symlink

- `O_EVTONLY` ⟶ eventOnly

- `O_CLOEXEC` ⟶ closeOnExec

The C constants for specify seek offsets map to Swift as follows:

- `SEEK_SET` ⟶ start

- `SEEK_CUR` ⟶ current

- `SEEK_END` ⟶ end

- `SEEK_HOLE` ⟶ nextHole

- `SEEK_DATA` ⟶ nextData

## See Also

### Adopting System

Adopting Swift File Operations

Migrate existing C code to Swift, using the file operations provided by the System module.

Adopting Swift Error Constants

Migrate existing C code to Swift, using the error constants provided by the System module.

