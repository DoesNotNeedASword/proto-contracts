# proto-contracts

Shared gRPC contracts for the voting pet project.

## Layout

- `proto/user/v1` contains user contracts.
- `proto/party/v1` contains party contracts.
- `proto/voting/v1` contains voting contracts.
- `gen/go` is the target directory for generated Go code.
- `openapi` is the target directory for generated REST/OpenAPI output.

## Generate

Install Buf, then run:

```powershell
buf dep update
buf lint
buf generate
```

If Buf is not installed, the same commands can be run through Go:

```powershell
go run github.com/bufbuild/buf/cmd/buf@latest dep update
go run github.com/bufbuild/buf/cmd/buf@latest lint
go run github.com/bufbuild/buf/cmd/buf@latest generate
```
