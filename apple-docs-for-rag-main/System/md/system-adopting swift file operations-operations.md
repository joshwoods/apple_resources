

- System
-  Adopting Swift File Operations 

Article

# Adopting Swift File Operations

Migrate existing C code to Swift, using the file operations provided by the System module.

## Overview

The C functions for file operations map to Swift as follows:

- `close` ⟶ close()

- `lseek` ⟶ seek(offset:from:)

- `open` ⟶ open(_:_:options:permissions:retryOnInterrupt:)

- `pread` ⟶ read(fromAbsoluteOffset:into:retryOnInterrupt:)

- `pwrite` ⟶ write(toAbsoluteOffset:_:retryOnInterrupt:)

- `read` ⟶ read(into:retryOnInterrupt:)

- `write` ⟶ write(_:retryOnInterrupt:)

## See Also

### Adopting System

Adopting Swift File Options

Migrate existing C code to Swift, using the file-operation options provided by the System module.

Adopting Swift Error Constants

Migrate existing C code to Swift, using the error constants provided by the System module.

