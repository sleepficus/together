# Source provenance

This candidate exports the newer Together application working tree. All 181 selected original files (5,499,784 bytes) match the October 12 frozen source archive. The original Git HEAD is `2e03e0809f50c45eca8bd0c541137ebe5ee3496b` plus uncommitted application changes, so HEAD alone does not identify these bytes. The original selected-byte manifest was `c12e98c3504a70693e4fe62cce54091c7f037958f221a833b57cc966f3ec8285`.

This interface was filmed locally. The existing hosted demonstration still serves October 4 Worker version `550da12a-b972-4069-9965-c6516d8d2d74`, tied by historical receipts to older app commit `2b1281ec6ee4cf57d3770f2977b98d62cd89bc24`. The October 14 preview is a separate deployment of the newer release, recorded in [HOSTED-VERIFICATION.md](HOSTED-VERIFICATION.md). The historical trial itself ran before the final October 4 correction; it is not a rerun on that final version.

Only application/build/test files were exported. Private records, credentials, operator activation/restore scripts, unrelated house/suit/research material and Git history were excluded. Together's own agent adapters, conversation and work integration remain. Deployment targets and host allowlists were sanitized; corresponding config fixture names were updated. New installation helpers and public documentation were added. Inline contributor credits remain; private journey/notebook links were removed. The backup panel now states that restore automation is excluded. A browser-discovered routing bug was repaired by decoding the conversation path ID once; encoded-ID, invalid-encoding and audience/authentication regressions were added.

Package scripts expose one-command local start/smoke and explicit Cloudflare build/dry-run/deploy. Optional OAuth/MCP configuration requires its own setup, is disabled by default and has no Artifacts binding. The initial packaging did not deploy or publish the app. A separate October 14 preview was subsequently deployed. Steve authorized making the standalone repository public on October 14.

The install prerequisite is Node.js 22.13+ because the local server uses unflagged built-in SQLite. Package and lockfile root engines agree; checks ran on Node 22.23.1.

## GitHub preparation — October 14, 2026

Prepared from the verified private candidate ZIP SHA-256 `e035b66d8df6cbb5770767ba71934edf74afc576a690606421f3e5ec60adbb44`. Steve requested upload, description, installation/use instructions and hackathon compliance, with the repository kept private. Added MIT LICENSE, repository metadata and updated documentation. Application code was unchanged from that candidate at the initial repository commit `e8cc8790b0cb6df1359a746af02bdc3c5efa4e7f`. The source manifest is refreshed for these packaging/documentation changes. Steve approved Tempo’s r3 video; no video or private recording is included.

## Hosted closure — October 14, 2026

Runtime commit `21a11cf557c0e44c5d7b2c134b8c2edffc2a8736` adds one login-page fix and its regression tests to the initial repository release. A native Safari form exposed an origin rejection that explicit-origin API probes had missed. The login page now uses the `same-origin` referrer policy; null and foreign origins remain rejected. Documentation updates after this runtime commit do not change deployed application behavior. The source manifest covers the current checkout.
