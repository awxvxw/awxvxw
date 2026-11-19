# Pocket AI Android build status

Repository: https://github.com/awxvxw/awxvxw

The GitHub Actions workflow builds Alibaba's official MNN Android chat app for arm64-v8a, adds the MNN-Pocket-0.3B-MNN files as built-in model assets, and uploads the resulting debug APK as a workflow artifact.

Model source: https://huggingface.co/taobao-mnn/MNN-Pocket-0.3B-MNN

The model card documents five files: `llm.mnn`, `llm.mnn.weight`, `llm_config.json`, `tokenizer.mtok`, and `config.json` (about 173 MB total).

Important: a successful workflow run and device-side inference test are still required before claiming the APK is ready. The model assets are placed into the upstream app's built-in model directory; the workflow verifies the model files are present in the APK archive.

Build workflow: Actions → Build Pocket AI Android APK → Run workflow.
