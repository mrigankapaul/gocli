# Go Comamnd
```
gocli
    - greetings
        - go.mod // generate using go mod init example.com/greetings
        - greetings.go
    - hello // hello package has a dependency on greetings package
        - go.mod // generate using go mod init hello. Add replace example.com/greetings => ../greetings to mod file
        - hello.go // has the main function that depends on greetings.
```

```
    cd hello
    go build
    go get example.com/greetings
    ./hello
    go run hello go.
    go run .
    go test -v
    go list -f '{{.Target}}' // to locate the install path // /Users/mrigankapaul/go/bin
    export PATH=$PATH:/Users/mrigankapaul/go/bin
    hello
```