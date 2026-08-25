Stable single-thread UCI release promoted from `v0.3.0-rc.1`.

- Release commit: `be272adfa0dcf796dc78e893f44396c7b8441c92`
- Frozen chess source: `c82c1cd59d83e4db2610b3954e3b377df30587ee`
- 5,000/5,000 no-recovery Fastchess games completed.
- UCI compliance passed before and after the burn-in.
- Against locked v0.2.0 at `5+0.05`: 48 W / 28 L / 24 D,
  +70.44 +/- 48.46 Elo, 99.84% LOS.
- Official Cute Chess 1.5.1 completed 2/2 games at repeating `40/15:00`
  without a time or protocol failure.
- Exact-tag CI and all four native release builds passed.

Recommended configuration: `Threads=1`, `Hash=256`, pondering off, external
common opening book. Use a generic build unless the target CPU is known to
support the Haswell/AVX2 build.

This release does not claim Stockfish parity, an official CCRL rating,
multi-thread strength, NNUE, or engine-side Syzygy.
