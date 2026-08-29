# Official Devstral Small 2 open-source scope

This repository preserves the unique artifacts directly published by Mistral AI for Devstral Small 2.

## Model distribution

- Upstream: `mistralai/Devstral-Small-2-24B-Instruct-2512`
- Host: Hugging Face
- Official size shown by Hugging Face: about 51.6 GB
- Official format: FP8 safetensors plus configuration, tokenizer, prompts and model documentation
- License metadata: Apache-2.0
- The entire pinned upstream file tree is mirrored byte-for-byte into GitHub Release assets.

The upstream model repository does not currently include a standalone `LICENSE` file. Its model-card metadata declares `apache-2.0`, and Mistral AI's Devstral 2 announcement states that Devstral Small 2 uses Apache 2.0. This provenance is retained in `UPSTREAM_LICENSE_NOTICE.txt` and this audit documentation.

## Official companion source

Mistral AI directly releases and recommends:

1. `mistralai/mistral-vibe` — native open-source coding-agent CLI released with Devstral 2.
2. `mistralai/mistral-common` — Mistral's official preprocessing/inference utility library referenced by the model.

Pinned source revisions:

- mistral-vibe: `50d99cf79b55ba92e43fa1ffdb0fc9c7bee83533`
- mistral-common: `208f15cf102c180363a489e96efc7b3bb8e5115b`

Their complete Git trees are stored under `official-source/`, with original Git blob SHA manifests and automated blob verification.

## Excluded from the official mirror scope

Third-party runtimes, IDE integrations, GGUF/community quantizations, adapters, finetunes and derivative models are not copied because they are not the unique official Devstral Small 2 source distribution published by Mistral AI.
