# Perp Protocol v1 (in dev)

## Local Development

To build parts of the project which use Anchor:

```sh
anchor build
# or
anchor build --arch sbf
```

To build the Rust program (from `/program`):

```sh
cargo build
```

## Deploy to Devnet

From the `/program` directory:

```sh
sh devnet_deploy.sh
```

## Tests

All tests are located in `/program/tests`.

To run all tests:

```sh
cargo test -- --show-output
```

```

---

**Summary of changes:**
- Used `##` for section headings.
- Clarified directory context for commands.
- Improved grammar and flow.

Let me know if you want this version applied to your `README.md`!
```
