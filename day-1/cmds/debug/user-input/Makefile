PHONY: run
run:
	go run main.go

.PHONY: debug
debug:
	dlv debug --build-flags="-gcflags='all=-N -l'"

.PHONY: debug-headless
debug-headless:
	dlv debug --headless --listen :9091 --api-version 2

.PHONY: connect-to-headless-delve
connect-to-headless-delve:
	dlv connect :9091