# Lane 1.4.136 recovery

Reconstructed from the saved 1.4.131 build with fixes132-135. This is not a byte-identical copy of135.

`1.4.136-patch.zip` contains complete helper source, compile-only SDK stubs, bootstrap classes, build scripts and tests. No separate signing keys, real provider credential source, tool jars, or APK files are included.

APK version:1.4.136, code336; size:123060057bytes.
SHA256:`112948e076ecee89369edd90b2cc3cbd723de7243ff22287fa8e239c2268563f`.

Rebuild requires Java17, Python3, saved base131 at `base/1.4.131.apk`, and tool jars from checkpoint124 at `tools/`. Run `python3 build136.py`, then `python3 verify_all.py`. The build script recovers signing material locally from the existing base APK.

Verified locally: original-class/method scope; update certificate and signature; ZIP/DEX integrity; native16KiB alignment; application method references; journal retention/redaction; database receiver/schema/header checks; player index bounds; coroutine forwarding contract fixtures. Phone installation, actual download completion and Android coroutine timing remain unverified.
