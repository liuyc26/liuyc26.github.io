+++
title = 'Built from scratch'
description = 'Re-implementing core infrastructure in Python to learn how it works: Redis, a DNS server, an HTTP server, a POSIX shell and an AI coding agent.'
weight = 5
cmd = 'make build-your-own'
stack = ['Python', 'Networking', 'Protocols']
[[links]]
  name = 'Redis'
  url = 'https://github.com/liuyc26/codecrafters-redis-python'
[[links]]
  name = 'DNS server'
  url = 'https://github.com/liuyc26/codecrafters-dns-server-python'
[[links]]
  name = 'HTTP server'
  url = 'https://github.com/liuyc26/codecrafters-http-server-python'
[[links]]
  name = 'Shell'
  url = 'https://github.com/liuyc26/codecrafters-shell-python'
[[links]]
  name = 'AI coding agent'
  url = 'https://github.com/liuyc26/codecrafters-claude-code-python'
+++

A series of CodeCrafters challenges where I rebuilt well-known tools from the protocol up:

- **Redis**: RESP protocol parsing, key expiry and core commands
- **DNS server**: parsing and building DNS packets, forwarding queries
- **HTTP server**: request parsing, routing, concurrent connections, compression
- **Shell**: builtins, PATH lookup, quoting, redirection
- **AI coding agent**: a minimal Claude Code-style agent loop with tool calls
