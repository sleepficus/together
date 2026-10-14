# Verification — October 14, 2026

This private candidate packages the newer Together interface for installation and review. The repository preparation uses MIT and targets the private sleepficus/together repository at Steve’s request. Public visibility, revised video and manual submission remain separate.

- Fresh `npm ci`: passed.
- Core tests: 465/465 passed. After the encoded task-discussion ID repair and private-link removal, the complete 465-test suite, typecheck and Cloudflare dry bundle passed. Browser-created work and task-discussion messages remained after a refresh.
- `npm run typecheck`: passed.
- `npm run check:cloud`: passed; protected assets, four SQLite Durable Objects and Artifacts binding bundled.
- `npm run smoke:local`: passed; fresh startup, occupied-port refusal, HTML/module delivery, authentication denials, cookie sign-in, live project read, logout and shutdown.

The newer candidate also passed a real in-app-browser check of automatic local sign-in, a newly created task, its discussion message and persistence after refresh. The pre-fix task discussion returned 404; the new regression reproduced that failure before repair. The narrow repair decodes only the conversation ID once, after existing authentication and membership checks; malformed encoding returns a controlled 400.

These checks ran on the same Mac using Node 22.23.1 and npm 10.9.8, with fresh isolated dependency trees and caches. A second-machine install, fresh Cloudflare provisioning, Git/Docker companion execution and connected-agent concurrency were not performed. Worker builds were dry runs; they did not replace the existing demonstration deployment. Fixture success does not establish measured collaboration benefit. Optional OAuth/MCP activation and recovery automation require separate setup; the private operator restore script is excluded.
