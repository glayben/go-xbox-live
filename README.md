# go-xbox-live

A Go client library for Xbox Live REST APIs, generated from the OpenAPI specification using [oapi-codegen](https://github.com/oapi-codegen/oapi-codegen).

## Installation

```bash
go get github.com/glayben/go-xbox-live
```

## Usage

```go
import "github.com/glayben/go-xbox-live/xboxlive"

client, err := xboxlive.NewClientWithResponses("https://your-xbox-live-endpoint")
```

The client provides typed methods for all Xbox Live API endpoints, including:

- **Presence** — online status, device and title activity
- **Profile & Social** — profile settings, people list, friends, followers, favorites, mute/avoid lists
- **Achievements** — by user and by title
- **Game Clips** — upload, delete, update, query
- **Leaderboards & Stats** — player stats and leaderboards
- **Multiplayer Sessions** — create, query, join, handles
- **Inventory & Entitlements** — user inventory
- **Title Storage** — global, trusted platform, untrusted platform, session-scoped blobs
- **Marketplace** — browse, search, content ratings, metadata
- **Reputation** — feedback submission, score reset
- **Messaging** — inbox and outbox
- **Permissions** — permission checks
- **System** — QOS servers, string validation

## Regenerate

To regenerate the client from the OpenAPI spec:

```bash
go generate ./...
```

Requires `api.yaml` (the OpenAPI specification, not included in the repository).

## License

MIT
