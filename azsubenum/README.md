# AzSubEnum 
https://github.com/yuyudhn/AzSubEnum

## Usage

**Build**
```
docker build -f Containerfile -t azsubenum .
```

**Run**
```
docker run --rm -it azsubenum
docker run --rm -it azsubenum --base mydomain.com --thread 10 --permutations permutations.txt
```
