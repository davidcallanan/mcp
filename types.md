# Types

## Bool

| Element | Size   | Values | Repr   |
|---------|--------|--------|--------|
| Value   | 1 byte | FALSE  | `0x00` |
|         |        | TRUE   | `0x01` |

## Short

| Element | Size    | Values            | Repr                    |
|---------|---------|-------------------|-------------------------|
| Value   | 2 bytes | -32,768 to 32,767 | Byte 0: `(value >> 8) % 256` |
|         |         |                   | Byte 1: `value % 256` |
