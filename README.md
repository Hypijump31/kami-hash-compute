# kami-hash-compute

[![KAMI Plugin](https://img.shields.io/badge/KAMI-plugin-8A2BE2)](https://github.com/Hypijump31/KAMI)
[![Signed](https://img.shields.io/badge/Ed25519-signed-green)](https://github.com/Hypijump31/kami-registry)

Compute SHA-256 or SHA-512 hash of any text.

## Install

```bash
kami install Hypijump31/kami-hash-compute@v0.1.0
```

## Usage

```bash
# SHA-256 (default)
kami exec dev.kami.hash-compute '{"text": "hello world"}'

# SHA-512
kami exec dev.kami.hash-compute '{"text": "hello world", "algorithm": "sha512"}'
```

## Arguments

| Name | Type | Required | Description |
|------|------|----------|-------------|
| `text` | string | yes | Text to hash |
| `algorithm` | string | no | `sha256` (default) or `sha512` |

## Build from source

```bash
git clone https://github.com/Hypijump31/kami-hash-compute
cd kami-hash-compute
kami build . --release
```

To also package as plugin.zip:

```bash
kami build . --release --package
```

## Security

- Filesystem: none
- Network: none
- Max memory: 16 MB
- Max execution: 1000 ms

## License

MIT
