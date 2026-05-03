# Docker build image

```powershell
$env:VERSION="3.7.7"

# Build với tag version
$env:VERSION="3.7.7"; docker build --no-cache --build-arg VERSION=$env:VERSION -t nqdev/omniroute:$env:VERSION .

# Tag latest
$env:VERSION="3.7.7"; docker tag nqdev/omniroute:$env:VERSION nqdev/omniroute:latest

# Push
$env:VERSION="3.7.7"; docker push nqdev/omniroute:$env:VERSION
docker push nqdev/omniroute:latest
```
