# Simple Server

This repo contains some very basic code to set up an HTTP server written in Elixir.

If you don't already have Elixir installed, please see [the Elixir website](https://elixir-lang.org/install.html) for installation instructions...

## Installation

* Clone the repo
```sh
git clone https://github.com/wesdunn/simpleserver-elixir.git && cd $_
```

* Download and install dependencies
```sh
mix deps.get
```

* Start the server...
```sh
iex -S mix
```

* Send some requests to the server (use another terminal window for this...)
Simple `GET` request
```sh
curl -v "http://localhost:8085/hello"
```

Simple `POST` request
```sh
curl -v -H 'Content-Type: application/json' "http://localhost:8085/post" -d '{"message": "hello world" }'
```

Ensure non-existant routes are handled properly
```sh
curl -v "http://localhost:8085/thisshouldbea404"
```


