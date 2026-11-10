# OGP models

Optional speech-to-text models for the Off Grid Pilot (OGP) Android app. The app ships with
Whisper base.en; this repo hosts the larger, more accurate **small.en** for pilots who want it.

## Install small.en on your phone

1. In the app: **Settings > Speech-to-text > small.en model (optional) > Get small.en**.
   Your browser downloads `ggml-small.en-q5_1.bin` (190 MB; Wi-Fi recommended).
2. Back in the app, tap **Import file** and pick the file in Downloads.
3. Choose small.en under **Model**. You can delete the file from Downloads afterwards.

No signal at the field? A pilot who has the file can send it to you with Quick Share.

## Files

| File | Size | SHA-256 |
|---|---|---|
| `ggml-small.en-q5_1.bin` (release `models-v1`) | 190,098,681 bytes | `bfdff4894dcb76bbf647d56263ea2a96645423f1669176f4844a1bf8e478ad30` |

The app checks this fingerprint before it uses the file.

## Source and license

Unmodified copy of `ggml-small.en-q5_1.bin` from
[ggerganov/whisper.cpp on Hugging Face](https://huggingface.co/ggerganov/whisper.cpp), a quantized
conversion of OpenAI's Whisper small.en. Whisper's weights and whisper.cpp are released under the
MIT License (see `LICENSE`).
