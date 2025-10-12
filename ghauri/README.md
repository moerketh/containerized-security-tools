# ghauri
https://github.com/r0oth3x49/ghauri

## Usage

**Build**
```
docker build -f Containerfile -t ghauri .
```

**Run**
```
docker run --rm -it ghauri
docker run --rm -it ghauri -u http://www.site.com/vuln.php?id=1 --dbs
docker run --rm -it -v $(pwd):/data ghauri -r /data/req.txt
```
