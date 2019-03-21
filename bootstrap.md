# Configure Laravel Bootstrap support
##### Current version 4.3.1

#### Edit package.json to update packages to the latest versions

```console
    "devDependencies": {
        ...
        "bootstrap": "^4.3.1",
        "jquery": "^3.3.1",
        "popper.js": "^1.14.7",
        ...
    }
}
```

#### Install all front-end packages

```console
npm install
```

#### Compile SCSS and Javascript files if they are modified

```console
npm run dev
npm run watch
```
