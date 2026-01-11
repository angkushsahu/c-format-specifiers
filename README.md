## C Format Specifiers

### Table of contents

1. [Integer Types](#1-Integer-Types)
1. [Floating Point Types](#2-Floating-Point-Types)
1. [Character and String Types](#3-Character-and-String-Types)
1. [Pointers](#4-Pointers)
1. [Booleans](#5-Booleans)
1. [Length Modifiers](#6-Length-Modifiers)
1. [Special / Literal Specifiers](#7-Special--Literal-Specifiers)

### 1. Integer Types

**Signed Integers**

| Data type             | Format specifier |
| --------------------- | ---------------- |
| `signed char`         | `%hhd`           |
| `short int`           | `%hd`            |
| `int`                 | `%d` or `%i`     |
| `long int`            | `%ld`            |
| `long long int` (C99) | `%lld`           |
| `int8_t`              | `%" PRId8 "`     |
| `int16_t`             | `%" PRId16 "`    |
| `int32_t`             | `%" PRId32 "`    |
| `int64_t`             | `%" PRId64 "`    |
| `intmax_t`            | `%" PRIdMAX "`   |
| `ptrdiff_t`           | `%td`            |

**Unsigned Integers**

| Data type                  | Format specifier |
| -------------------------- | ---------------- |
| `unsigned char`            | `%hhu`           |
| `unsigned short`           | `%hu`            |
| `unsigned int`             | `%u`             |
| `unsigned long`            | `%lu`            |
| `unsigned long long` (C99) | `%llu`           |
| `uint8_t`                  | `%" PRIu8 "`     |
| `uint16_t`                 | `%" PRIu16 "`    |
| `uint32_t`                 | `%" PRIu32 "`    |
| `uint64_t`                 | `%" PRIu64 "`    |
| `uintmax_t`                | `%" PRIuMAX "`   |
| `size_t`                   | `%zu`            |

**Integer Bases**

| Base            | Specifier |
| --------------- | --------- |
| Octal           | `%o`      |
| Hex (lowercase) | `%x`      |
| Hex (uppercase) | `%X`      |

### 2. Floating Point Types

| Data type     | Format specifier            |
| ------------- | --------------------------- |
| `float`       | `%f` *(promoted to double)* |
| `double`      | `%lf`                        |
| `long double` | `%Lf`                       |

**Variants**

| Meaning         | Specifier  |
| --------------- | ---------- |
| Scientific      | `%e`, `%E` |
| Shortest        | `%g`, `%G` |
| Hex float (C99) | `%a`, `%A` |

### 3. Character and String Types

| Data type                   | Format specifier |
| --------------------------- | ---------------- |
| `char`                      | `%c`             |
| `signed char` (as number)   | `%hhd`           |
| `unsigned char` (as number) | `%hhu`           |
| `char *` (string)           | `%s`             |
| `wchar_t`                   | `%lc`            |
| `wchar_t *`                 | `%ls`            |

### 4. Pointers

| Data type | Format specifier |
| --------- | ---------------- |
| `void *`  | `%p`             |

### 5. Booleans

| Data type       | Format specifier |
| --------------- | ---------------- |
| `_Bool`, `bool` | `%d`             |

### 6. Length Modifiers

| Modifier | Meaning       |
| -------- | ------------- |
| `hh`     | `char`        |
| `h`      | `short`       |
| `l`      | `long`        |
| `ll`     | `long long`   |
| `z`      | `size_t`      |
| `t`      | `ptrdiff_t`   |
| `j`      | `intmax_t`    |
| `L`      | `long double` |

### 7. Special / Literal Specifiers

| Specifier | Meaning                       |
| --------- | ----------------------------- |
| `%%`      | Print `%`                     |
| `%n`      | Store number of chars printed |
| `%*d`     | Suppress assignment (`scanf`) |
