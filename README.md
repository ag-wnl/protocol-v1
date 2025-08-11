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
cd program
cargo check
cargo test --lib -- --nocapture
cargo test -- --nocapture  # runs integration tests in program/tests

# specific flows:
cargo test -q test_perp_markets -- --nocapture
cargo test -q test_place_perp_order -- --nocapture
cargo test -q test_consume_events -- --nocapture

# start local validator
solana-test-validator --reset
solana config set --url http://127.0.0.1:8899
```

```

---

**Summary of changes:**
- Used `##` for section headings.
- Clarified directory context for commands.
- Improved grammar and flow.

Let me know if you want this version applied to your `README.md`!
```
