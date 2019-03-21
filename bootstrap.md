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
// run all mix tasks
npm run dev

// run all mix tasks and watch for changes
npm run watch

// run all mix tasks and minify output
npm run production
```

#### Create the HTML page - resources/views/welcome.blade.php

```html
<!doctype html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
        <meta name="description" content="">
        <meta name="author" content="">
        <title>Cover Template for Bootstrap</title>
        <link rel="icon" href="../../../../favicon.ico">
        <link href="{{asset('css/app.css')}}" rel="stylesheet">
        <link href="{{asset('css/custom.css')}}" rel="stylesheet">
    </head>

    <body class="text-center">
        <div class="cover-container d-flex w-100 h-100 p-3 mx-auto flex-column">
            <header class="masthead mb-auto">
                <div class="inner">
                    <h3 class="masthead-brand">Cover</h3>
                    <nav class="nav nav-masthead justify-content-center">
                        <a class="nav-link active" href="#">Home</a>
                        <a class="nav-link" href="#">Features</a>
                        <a class="nav-link" href="#">Contact</a>
                    </nav>
                </div>
            </header>

            <main role="main" class="inner cover">
                <h1 class="cover-heading">Example Page</h1>
                <p class="lead">This is an example of Bootstrap 4.3.1</p>
                <p class="lead">
                    <a href="#" class="btn btn-lg btn-secondary">Learn more</a>
                </p>
            </main>

            <footer class="mastfoot mt-auto">
                <div class="inner">
                    <p>&copy; 2017-2018 Company, Inc. &middot; <a href="#">Privacy</a></p>
                </div>
            </footer>
        </div>

        <script src="{{asset('js/app.js')}}"></script>
    </body>
</html>
```

#### Create the custom CSS file - public/css/custom.css

```css
a,
a:focus,
a:hover {
  color: #fff;
}

.btn-secondary,
.btn-secondary:hover,
.btn-secondary:focus {
  color: #333;
  text-shadow: none;
  background-color: #fff;
  border: .05rem solid #fff;
}

html,
body {
  height: 100%;
  background-color: #333;
}

body {
  display: -ms-flexbox;
  display: flex;
  color: #fff;
  text-shadow: 0 .05rem .1rem rgba(0, 0, 0, .5);
  box-shadow: inset 0 0 5rem rgba(0, 0, 0, .5);
}

.cover-container {
  max-width: 42em;
}

.masthead {
  margin-bottom: 2rem;
}

.masthead-brand {
  margin-bottom: 0;
}

.nav-masthead .nav-link {
  padding: .25rem 0;
  font-weight: 700;
  color: rgba(255, 255, 255, .5);
  background-color: transparent;
  border-bottom: .25rem solid transparent;
}

.nav-masthead .nav-link:hover,
.nav-masthead .nav-link:focus {
  border-bottom-color: rgba(255, 255, 255, .25);
}

.nav-masthead .nav-link + .nav-link {
  margin-left: 1rem;
}

.nav-masthead .active {
  color: #fff;
  border-bottom-color: #fff;
}

@media (min-width: 48em) {
  .masthead-brand {
    float: left;
  }
  .nav-masthead {
    float: right;
  }
}

.cover {
  padding: 0 1.5rem;
}
.cover .btn-lg {
  padding: .75rem 1.25rem;
  font-weight: 700;
}

.mastfoot {
  color: rgba(255, 255, 255, .5);
}
```
