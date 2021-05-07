# truncate white space

Truncate a string at a certain length, using the closest whitespace character.

## Usage

Add the following to your `Cargo.toml`

```toml
truncate_string_at_whitespace = "1.0.2"
```

Then

```rust
use truncate_string_at_whitespace::truncate_text;


fn main () {
  let s = "This is a string that I want to truncate";
  let st = truncate_text(s, 12);
  assert_eq!(st, "This is a");
  let st2 = truncate_text(s, 16);
  assert_eq!(st2, "This is a string");
}
```

## Licence
© 2021 Todd Kennedy, Apache-2.0
