Stockfish.js 18.0.8 corresponding-source inputs for the unmodified lite single Worker.

Upstream: https://github.com/nmrugg/stockfish.js
Exact npm gitHead: 93c994592dcf3b4b21052ab925e9b534df9c0918
Source archive URL: https://codeload.github.com/nmrugg/stockfish.js/zip/93c994592dcf3b4b21052ab925e9b534df9c0918
Source archive SHA256: 59d67bb0468e7c4464ea475b1631a3b2e8b99751c01a71a9e5de82200e422202
NNUE URL: https://tests.stockfishchess.org/api/nn/nn-9067e33176e8.nnue
NNUE SHA256: 9067e33176e8c5edb7aa8db6a3aedd012f84a1f39872e86357c6c2d0993f314d

License: GNU GPL v3; see Copying.txt inside the archive and GPL-3.0.txt next to the Worker.
The source archive is downloaded from the exact upstream commit without modification.
The additional network is the one named by src/lite_nets.h, verified by SHA256.

Build instructions (Linux or a compatible Unix build environment):
1. Extract stockfish-18.0.8-source.zip.
2. Copy nn-9067e33176e8.nnue into the extracted source's src/ directory.
3. Install the general-purpose toolchain described by upstream: Emscripten 3.1.7,
   Node.js, GNU Make, Python and normal C/C++ build prerequisites.
4. Run: node build.js --single-threaded --lite -f
5. Compare behavior with the supplied Worker. The project's SHA256SUMS identifies
   the exact unmodified npm binaries we serve; a bit-for-bit rebuild is not claimed.

The source files, network, build script and vendored JavaScript minifier sources
are supplied here. General-purpose compiler tools are not bundled.
No rebuild using Emscripten has been executed in this Windows environment.
This is technical provenance, not a legal determination about the enclosing site.
