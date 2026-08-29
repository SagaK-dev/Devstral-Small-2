# Devstral Small 2 mirroring design

The official checkpoint is too large for normal Git objects, so model files are stored in GitHub Releases.

## Model mirror

Each pinned upstream file is downloaded byte-for-byte. Files larger than 1.5 GB are split into deterministic ordered assets.

Per-file manifests record:

- original upstream path
- exact upstream revision
- original size
- calculated SHA-256
- upstream SHA-256 where Hugging Face/Xet exposes it
- ordered Release asset names and sizes

The final verifier checks every upstream path, every part size, reconstructed file sizes and all available upstream SHA-256 digests.

## License metadata

The model-card metadata declares Apache-2.0, but the pinned Hugging Face model tree has no standalone LICENSE file. A separate `UPSTREAM_LICENSE_NOTICE.txt` is therefore stored as mirror provenance and is not counted as an upstream model file.

## Official source mirror

The complete pinned Git trees for `mistralai/mistral-vibe` and `mistralai/mistral-common` are copied under `official-source/`. Their source tree manifests retain original Git blob SHA values and an Actions job verifies copied file contents against those blob hashes before committing.
