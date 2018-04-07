# About

## Docs [wiki](https://docs.npmjs.com/cli/ls)

### Query pakages
```
npm ls --global=true --depth=0
```

### Config proxy
```
npm get proxy

npm set proxy=http://{domain}%5C{username}:{mypassword}@{proxyip}:{port}/
npm config rm proxy

npm set https-proxy=https://{domain}%5C{username}:{mypassword}@{proxyip}:{port}/
npm config rm https-proxy

npm config set strict-ssl false

npm config get registry
```