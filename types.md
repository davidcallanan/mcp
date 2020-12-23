# Types

## Bool

| Element | Size   | Values | Repr   |
|---------|--------|--------|--------|
| Value   | 1 byte | FALSE  | `0x00` |
|         |        | TRUE   | `0x01` |

## Short

| Element | Size    | Values            | Repr                                |
|---------|---------|-------------------|-------------------------------------|
| Value   | 2 bytes | -32,768 to 32,767 | Byte 0: `(value >> (8 * 1)) & 0xFF` |
|         |         |                   | Byte 1: `(value >> (8 * 0)) & 0xFF` |

## Int

| Element | Size    | Values                          | Repr                                |
|---------|---------|---------------------------------|-------------------------------------|
| Value   | 4 bytes | -2,147,483,648 to 2,147,483,647 | Byte 0: `(value >> (8 * 3)) & 0xFF` |
|         |         |                                 | Byte 1: `(value >> (8 * 2)) & 0xFF` |
|         |         |                                 | Byte 2: `(value >> (8 * 1)) & 0xFF` |
|         |         |                                 | Byte 3: `(value >> (8 * 0)) & 0xFF` |

## Long

| Element | Size    | Values                                                  | Repr                                |
|---------|---------|---------------------------------------------------------|-------------------------------------|
| Value   | 8 bytes | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | Byte 0: `(value >> (8 * 7)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 1: `(value >> (8 * 6)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 2: `(value >> (8 * 5)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 3: `(value >> (8 * 4)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 4: `(value >> (8 * 3)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 5: `(value >> (8 * 2)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 6: `(value >> (8 * 1)) & 0xFF` |
| Value   | 8 bytes |                                                         | Byte 7: `(value >> (8 * 0)) & 0xFF` |
