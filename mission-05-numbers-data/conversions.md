# Mission 5 — Number representation and text encoding

## Task 5.1 — Manual conversions

### Decimal 13 to binary

Divide repeatedly by 2 and record the remainders:

```text
13 ÷ 2 = 6 remainder 1
 6 ÷ 2 = 3 remainder 0
 3 ÷ 2 = 1 remainder 1
 1 ÷ 2 = 0 remainder 1
```

Read the remainders from bottom to top: `13₁₀ = 1101₂`.

### Decimal 25 to binary

```text
25 ÷ 2 = 12 remainder 1
12 ÷ 2 =  6 remainder 0
 6 ÷ 2 =  3 remainder 0
 3 ÷ 2 =  1 remainder 1
 1 ÷ 2 =  0 remainder 1
```

Read the remainders from bottom to top: `25₁₀ = 11001₂`.

### Binary 1010 to decimal

```text
1×2³ + 0×2² + 1×2¹ + 0×2⁰
= 8 + 0 + 2 + 0
= 10
```

Therefore, `1010₂ = 10₁₀`.

### Binary 1101 to decimal

```text
1×2³ + 1×2² + 0×2¹ + 1×2⁰
= 8 + 4 + 0 + 1
= 13
```

Therefore, `1101₂ = 13₁₀`.

### Hexadecimal A to decimal

Hexadecimal digit `A` has value 10, so `A₁₆ = 10₁₀`.

### Hexadecimal 1F to decimal

```text
1×16¹ + F×16⁰
= 1×16 + 15×1
= 31
```

Therefore, `1F₁₆ = 31₁₀`.

### Binary 1111 to hexadecimal

Group the four bits as one nibble. `1111₂` has value `8 + 4 + 2 + 1 = 15`; hexadecimal digit 15 is `F`. Therefore, `1111₂ = F₁₆`.

## Task 5.2 — Python built-in verification

The expressions below were evaluated in Python 3.9.6 interactive mode. For binary values, `int(value, 2)` parses a base-2 string; `[2:]` removes the `0b` prefix from `bin()`. For hexadecimal, `int(value, 16)` parses base 16, and `hex()` returns a string beginning with `0x`.

| Expression | Python result | Manual answer | Match |
| --- | ---: | ---: | --- |
| `bin(13)[2:]` | `1101` | `1101₂` | Yes |
| `bin(25)[2:]` | `11001` | `11001₂` | Yes |
| `int("1010", 2)` | `10` | `10₁₀` | Yes |
| `int("1101", 2)` | `13` | `13₁₀` | Yes |
| `hex(10)[2:].upper()` | `A` | `A₁₆` | Yes |
| `int("1F", 16)` | `31` | `31₁₀` | Yes |
| `hex(int("1111", 2))[2:].upper()` | `F` | `F₁₆` | Yes |

## Task 5.4 — Text encoding

- ASCII decimal code for uppercase `A`: `65`
- ASCII decimal code for lowercase `a`: `97`
- An example character outside basic ASCII: `€` (the euro sign)

Text encoding assigns numeric values to characters so computers can store and exchange text as data. Basic ASCII covers a limited set of characters; Unicode encodings such as UTF-8 allow many more characters, including `€`, to be represented.
