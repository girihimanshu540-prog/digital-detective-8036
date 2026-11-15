# Mission 5 — Numbers and Data

## 1. Task / objective
Convert between decimal, binary and hexadecimal, verify with Python,
build a converter, and explain text encoding.

## 2. Work completed

### Task 5.1 — Manual conversions

| Question | Answer |
|----------|--------|
| Decimal 13 to binary | 1101 |
| Decimal 25 to binary | 11001 |
| Binary 1010 to decimal | 10 |
| Binary 1101 to decimal | 13 |
| Hexadecimal A to decimal | 10 |
| Hexadecimal 1F to decimal | 31 |
| Binary 1111 to hexadecimal | F |

### Task 5.2 — Python verification

| Expression tested | Result | Matches my manual answer? |
|-------------------|--------|---------------------------|
| `bin(13)` | `0b1101` | Yes, apart from the `0b` prefix |
| `bin(25)` | `0b11001` | Yes, apart from the `0b` prefix |
| `int("1010", 2)` | `10` | Yes |
| `int("1101", 2)` | `13` | Yes |
| `int("A", 16)` | `10` | Yes |
| `int("1F", 16)` | `31` | Yes |
| `hex(int("1111", 2))` | `0xf` | Yes, apart from the `0x` prefix and lowercase `f` |

### Task 5.3 — Number converter

The program asks the user to type a decimal number. `input()` returns that
number as text, so `int()` converts it into an integer. The program then
passes the integer to `bin()` to get the binary version and to `hex()` to
get the hexadecimal version, and prints both results.

- `bin()` takes an integer and returns its binary form as a string that
  starts with the prefix `0b`.
- `hex()` takes an integer and returns its hexadecimal form as a string
  that starts with the prefix `0x`.
- The typed text must be converted with `int()` first, because `input()`
  gives a string, and `bin()` and `hex()` only work on numbers.

| Test number | Binary output | Hexadecimal output |
|-------------|---------------|--------------------|
| 10 | 0b1010 | 0xa |
| 100 | 0b1100100 | 0x64 |
| 255 | 0b11111111 | 0xff |

### Task 5.4 — Text encoding
- ASCII code for A and a: `A` is 65 and `a` is 97 (found using `ord("A")` and `ord("a")`).
- Why an encoding standard is needed: a computer can only store numbers, so
  each character has to be given a number. An encoding standard such as
  ASCII or UTF-8 is an agreed list of these numbers, so every computer
  turns the same stored number back into the same letter.
- A character outside basic ASCII: the rupee sign ₹. Its code is 8377, which
  is far beyond ASCII's range, so it needs UTF-8. (`é` and emoji also work.)

## 3. Commands / tools used
(`python3`, the interactive shell, `input()`, `int()`, `bin()`, `hex()`,
`ord()`, with the purpose of each.)

