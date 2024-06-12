## Date Created

12 June 2024

# python-docker

Containerizing a simple fastapi Python app. 

## Colima 
### Why Colima over Docker Desktop?

Colima is an open-source project, offering transparency and community contributions. It provides more customization options for the virtual machine environment and has no licensing restrictions unlike Docker Desktop. Additionally, Colima supports different container runtimes like Docker and Containerd, giving us the flexibility to choose the best tool for our needs.

### Setting up Colima on macOS

To use Colima for container runtime on macOS, install it using Homebrew:

```bash
brew install colima
```

Start Colima with:

```bash
colima start
```

For a detached session:

```bash
colima start -d
```

Check the status of Colima:

```bash
colima status
```

Stop Colima when you’re done:

```bash
colima stop
```

For more detailed usage and options, please look to the Colima documentation.

## Containerization
### Run the application

```bash
docker compose up --build
```

### Run the application in the background

You can run the application detached from the terminal by adding the `-d` option

```bash
docker compose up --build -d
```


### Stop application

```bash
docker compose down
```

## Author

Selman Karaosmanoglu

## Credits

[Docker's Python Language Guide](https://docs.docker.com/language/python).

Colima’s GitHub Repository.