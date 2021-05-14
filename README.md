# GO - Bookings and Reservations

This is the repository for my bookings and reservations project.

- Built in Go version 1.16
- Uses the [chi router](https://github.com/go-chi/chi) for middleware routes
- Uses [alex edwards SCS](https://github.com/alexedwards/scs/) session management
- Uses [nosurf](https://github.com/justinas/nosurf) for CSRF Token POST Protection
- Uses [govalidator](https://github.com/asaskevich/govalidator) for validation

## Build

```shell
go build .
```

## Run

```shell
go run cmd/web/*.go
```

## Test

**run simple test**

```shell
go test
```

**run simple test verbose**

```shell
go test -v
```

**run test with coverage**

```shell
go test -cover
```

**run test with coverage and print result in html**

```shell
go test -coverprofile=coverage.out && go tool cover -html=coverage.out
```