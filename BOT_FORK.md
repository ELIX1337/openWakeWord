# Bot ONNX packaging fork

This fork packages the Python code from upstream openWakeWord 0.6.0 for Bot.
The source baseline is upstream tag v0.6.0, commit
`c8ef6912c5feccf1037b852d9bc6c7ed644135ba`. The published PyPI source
archive SHA-256 is `36858d90f1183e307485597a912a4e3c3384b14ea9923f83feaffae7c1565565`.
The upstream wheel SHA-256 is
`6f423a4e3ae9dd0e3cd12b50ff8abf69679f687b4ab349d7c82c021c0e2abc9d`.

The distribution is named `bot-openwakeword`, but the Python import remains
`openwakeword`. The only dependency change moves Linux `tflite-runtime` to the
optional `tflite` extra. Bot uses ONNX; TFLite is not installed by default.
The fork does not claim to track or contain upstream fixes automatically.

The upstream code is Apache-2.0, as stated in LICENSE. Pretrained model assets
have separate license restrictions and are not included in the wheel.
