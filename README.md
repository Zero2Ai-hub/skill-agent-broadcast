# skill-agent-broadcast

Cross-group signal router for OpenClaw. Broadcast one message to multiple Telegram/Discord group sessions simultaneously — for cross-agent coordination, alerts, and announcements.

## Usage

```bash
# Broadcast to named groups
node scripts/broadcast.js --message "Deploy complete!" --groups "github-ops,amazon-ops"

# Broadcast to all registered groups
node scripts/broadcast.js --message "⚡ System alert" --groups all

# Use raw Telegram chat IDs
node scripts/broadcast.js --message "Hello" --groups "-1003871838436,-1003578613620"

# Custom delay between sends
node scripts/broadcast.js --message "Update" --groups all --delay 1000
```

## Requirements

- Node.js
- OpenClaw gateway running with configured group sessions

## Install

```bash
npm install
```

## Part of the [Zero2Ai-hub](https://github.com/Zero2Ai-hub) skills ecosystem.
