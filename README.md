# Example .NET Core application for Docker

This is just example application, generated with
```
dotnet new webapp -n MyWebapp
```

Just added a [Dockerfile](Dockerfile).

## Building

```
docker build -t my-dotnet-web-app:1.0 .
```

Use any name or tag instead of `my-dotnet-web-app:1.0`, of course.

## Running

```
docker run --rm -it -p:80  my-dotnet-web-app:1.0
```

This will run in synchronous mode. Pressing `CTRL-C`  will stop and remove the container.

Appication will be exposed on random port.