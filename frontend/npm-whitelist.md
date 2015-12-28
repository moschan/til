# npm White List

## Problem
npm has `.npmignore`. But, this funciton is like **blacklist**. If you forgot to add filename that is you wana ignore from npm registry, that is published.

## Solution
If you want to ignore to file using **whitelist** method, you can use "files" propaty in `package.json` like a below:

```
{
  "files": [
    "README.md",
    "index.js",
    "package.json",
  ],
}
```

