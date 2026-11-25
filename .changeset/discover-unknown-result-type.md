---
'@modelcontextprotocol/client': patch
---

The connect-time `server/discover` probe no longer accepts a reply whose `resultType` is anything other than `complete`. Such a reply is now treated as unrecognized (the legacy `initialize` fallback, or a typed error when no fallback is allowed) instead of being used as the server's capabilities.
