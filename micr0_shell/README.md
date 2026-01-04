# micr0_shell 
https://github.com/senzee1984/micr0_shell.git

## Usage

**Build**
```
docker build -f Containerfile -t micr0_shell .
```

**Run**
```
docker run --rm -it micr0_shell
docker run --rm -it micr0_shell --ip 10.10.14.245 --port 4444 --language csharp
```
