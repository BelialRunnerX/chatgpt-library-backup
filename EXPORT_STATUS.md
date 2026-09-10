# Export Status

Snapshot target: ChatGPT Library as of 2026-09-10.

## Repository initialization

The repository was initialized successfully and is writable through the connected GitHub integration.

## Verified baseline export

A previously generated split Library export from 2026-09-07 represents 474 source entries. Its seven standalone ZIP parts are all under 25,000,000 bytes and are indexed in `archive/Condensed_Library_2026-09-07_PART_INDEX.txt`.

Library file references for the seven parts:

- Part 01: `file_00000000c1fc81fd9d389a670985832b` — 17,128,346 bytes
- Part 02: `file_00000000647481fd89154227ddc84488` — 21,843,259 bytes
- Part 03: `file_00000000488081fdaafa5a2f80a0105e` — 22,920,588 bytes
- Part 04: `file_0000000014a481fdb1c0fef30e006cec` — 15,018,435 bytes
- Part 05: `file_000000006b1881fdbd419fdb32100f9a` — 20,911,180 bytes
- Part 06: `file_00000000215481fdbb7e7e2279b2692b` — 21,266,464 bytes
- Part 07: `file_000000009ce081fdb95a285b6a500644` — 18,687,554 bytes

The older one-file combined archive `Condensed_Library_2026-09-07.zip` is 137,706,130 bytes and therefore exceeds GitHub's normal 100 MiB file limit; the seven-part set is the appropriate Git representation.

## Post-baseline delta

The Library contains substantial newer material created after the split export, including Sixth Edition expansion files, SkeletonKey and Mechanical Depth checkpoints, production/merge packages, visual implementation packs, and generated visual assets from 2026-09-08 through 2026-09-10. These newer entries must be included in the final current snapshot rather than treating the 2026-09-07 archive as complete.

## Connector limitation encountered

The connected GitHub write interface can create/update UTF-8 files and Git blobs when their full content is supplied directly, but it does not accept a ChatGPT Library file reference or a mounted local binary file path as an upload source. That prevents direct streaming of multi-megabyte ZIP, PDF, PNG/JPEG, and other binary Library objects from the Files connector into GitHub in this chat session.

Accordingly, this repository is **initialized and indexed but not yet a complete binary backup**. Do not treat the presence of this status file or the baseline index as confirmation that all Library bytes have been transferred.
