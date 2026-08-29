# Devstral Small 2 official mirror

This repository archives the official open-source/open-weight artifacts directly published by Mistral AI for Devstral Small 2.

## Canonical model

- Hugging Face: `mistralai/Devstral-Small-2-24B-Instruct-2512`
- Model family: Devstral Small 2
- Parameters: 24B
- Official weight format: FP8
- License metadata: Apache-2.0
- Approximate upstream size: 51.6 GB

## Official companion OSS

The repository also preserves pinned source snapshots of Mistral AI projects directly referenced for Devstral Small 2:

- `mistralai/mistral-vibe` — Mistral's native coding-agent CLI released for Devstral
- `mistralai/mistral-common` — Mistral's official preprocessing/inference utility library

Third-party runtimes and community quantizations are not copied into the official mirror scope.

## Storage

Large model files are stored as split GitHub Release assets. The original upstream path, size, SHA-256 (where supplied by Hugging Face/Xet), and ordered part list are preserved in manifests.

A model mirror is only marked complete after all pinned upstream files and Release part sizes have been verified.
