# Pelagion one-shot qualification profile

Use Windows 11 x64, a dedicated cache and current process account.
Keep the allowed workspace, runtime path and cache path explicit and
separate. Admission fails on an incompatible canonical cache. Verify
that unrelated processes and prior artifacts survive each run.

Build on the designated host with MSYS2 CLANG64, C/C++ compiler and
GNU make. Record toolchain, source commit, vendored identities and
archive notices. Build the minimal production cbm target twice with
TEST_SEAMS disabled. A verified executable and identity file are
local inputs. This profile configures no UI, daemon or agent client.

Set watcher_enabled, auto_watch and auto_index to false and use
index_max_files=4096, index_max_source_mb=32 and CBM_WORKERS=1.
Set CBM_ALLOWED_ROOT, CBM_CACHE_DIR and CBM_RUNTIME_DIR to the
explicit owned workspace, cache and runtime locations.

Only setup may invoke index_repository on the retained fixture.
The Pelagion consumer uses search_code with literal text and
get_code_snippet with an exact qualified name and no neighbors.
Limit one request to 20 raw rows or 40 source lines, 64 KiB stdout
and a finite deadline. Pelagion verifies bytes against the admitted
source manifest and owns the Windows process Job. Graph queries,
relationship queries, impact, indexing and configuration have no
agent dispatch in this profile.

Require unchanged source and agent settings, exact fixture and
artifact hashes, and no residual owned CBM process after success,
failure and cancellation. A relationship capability stays disabled
until its actual retained case and review qualify it. The build,
search, process and licence receipts are separate from this profile.
