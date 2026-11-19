# Pocket AI for Android

A local-first Android chat app for the MNN-Pocket-0.3B-MNN model.

## Goal
- Android APK targeting arm64-v8a.
- Bundle the MNN-Pocket model assets inside the APK.
- Run inference locally with Alibaba MNN; no network required for chat.
- Chinese chat UI, conversation history, clear-chat action.

## Model
Source: https://huggingface.co/taobao-mnn/MNN-Pocket-0.3B-MNN
The model card lists five runtime files: llm.mnn, llm.mnn.weight, llm_config.json, tokenizer.mtok, and config.json (about 173 MB total).

## Build status
Project initialization only. A working APK is not yet available. The Android runtime integration and reproducible build must pass before a release is published.

## License
The app code in this repository is Apache-2.0 unless otherwise noted. The model and MNN runtime retain their upstream licenses.


Build workflow updated to use the runner-provided Android SDK and install only required SDK packages.
