# JoobQ SDK for Go

A thin worker and producer client for the JoobQ SDK gateway of a self-hosted JoobQUI server: register jobs and
workflow blueprints, run their tasks with retries, heartbeats and graceful shutdown, and enqueue jobs (up to 500 in one
call with `EnqueueMany`) or start workflows. With JoobQ Pro on the server: batches with completion callbacks (`CreateBatch`,
`GetBatch`) and a shared sliding-window rate limit (`RateLimit`).
JoobQUI version 0.7.2; an SDK talks to a server of its own version or later.

- Requirements: Go 1.22 or newer; standard library only.
- Install: `go get github.com/azutoolkit/joobq-sdk-go`.
- Use: the module `github.com/azutoolkit/joobq-sdk-go`.
- Connect: the server's origin and its SDK token, read by the examples from `JOOBQ_GATEWAY_URL` and `JOOBQ_SDK_TOKEN`.
- Documentation: https://www.joobq.io/docs/develop/ (workers, jobs, workflows, the gateway contract).

More about JoobQ: https://www.joobq.io

## License

MIT (see `LICENSE`).
