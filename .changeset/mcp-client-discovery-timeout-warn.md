---
"agents": patch
---

Log `MCPClientManager` discovery timeouts at `warn` instead of `error`, and tag them with `reason: "timeout"` in `MCPDiscoveryResult` and `MCPDiscoverResult` so callers can distinguish recoverable timeouts from genuine failures without scraping console output.
