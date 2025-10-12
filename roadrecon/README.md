# ROADRecon
See: https://github.com/dirkjanm/roadtools


## Usage

**Build**
```
docker build -f Containerfile -t roadrecon .
```

**1. Authenticate**
```powershell
docker run --rm -it -v ${PWD}/roadrecon_data:/app/roadrecon_data roadrecon auth -u user@tenant.onmicrosoft.com
```

**2. Gather data**

PowerShell
```powershell
docker run --rm -it -v ${PWD}/roadrecon_data:/app/roadrecon_data roadrecon gather
```

Bash
```bash
docker run --rm -it -v $(pwd)/roadrecon_data:/app/roadrecon_data roadrecon gather
```

The error sqlalchemy.exc.OperationalError: (sqlite3.OperationalError) unable to open database file is a classic SQLite issue, often triggered in Docker by volume mounts. Try to restart the container runtime.

**3. Run GUI**

PowerShell
```powershell
docker run --rm -d -p 5001:5001 -v ${PWD}/roadrecon_data:/app/roadrecon_data roadrecon gui
```

Bash
```bash
docker run --rm -d -p 5001:5001 -v $(pwd)/roadrecon_data:/app/roadrecon_data roadrecon gui
```

Access at http://localhost:5001 from your host.