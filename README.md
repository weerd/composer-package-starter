# PHP Composer Package Starter Example


## Usage

Download this repository as a zip file without the Git history, rename it, run `git init` to initialize an empty git repository and then get cracking creating your own package.

You will need to update the following items with your package's name and info:

- rename the main repository directory
- README.md
- composer.json (package name, psr-4 namespaces, etc)
- tests/TestCase.php (rename the database table)
- tests/ExampleTest.php (rename)

If initially using the package locally, required by another local package make sure this package has been initialized as a git repository and make an initial commit, otherwise composer will not be able to install the package as a local vendor package.

Additionally, if initially using the package locally, add the following to the other project's **composer.json**:

```javascript
"repositories": [
    {
        "type": "vcs",
        "url": "../path/to/example-package"
    }
],
"require": {
    "weerd/example-package": "dev-master"
}
````

## Extras

_The `illuminate/database` package is required for development testing, however if this package is intended to be a Laravel package and/or a package that needs database transactions, feel free to move `illuminate/database` from `require-dev` to `require`._
