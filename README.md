# Zstandard - llm port

Original project: [Zstandard](https://github.com/facebook/zstd), version 1.5.7.
Original authors: Yann Collet, Meta Platforms, Inc. and the Zstandard contributors. [Original repository](https://github.com/facebook/zstd).

The library is the work of its original authors, not a product of llm-build-system.
This repository only maintains its llm build integration and source subset.
It is not an official upstream release. Upstream source and header files are
unchanged. Build configuration files added by this port are kept separately.
Upstream build systems, command-line tools, tests and manuals are omitted.

The original license is preserved verbatim in [LICENSE](LICENSE).
[Upstream license](https://github.com/facebook/zstd/blob/v1.5.7/LICENSE). Copyright and per-file license notices
remain in the original files.

Additional upstream copyright and license notices from the included source
files are reproduced verbatim in [NOTICE](NOTICE) for binary redistribution.
The original notices remain in the source files.

Build the static library with `llm build --release`. Consumers include
`<zstd.h>`, `<zstd_errors.h>` or `<zdict.h>`. This port uses the upstream
BSD license, portable C implementations and multithreaded compression.
Optional assembly and historical legacy-format decoders are not included.
