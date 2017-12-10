# PHP Composer Package Starter Example


## Usage

Download this repository as a **zip** file without the Git history, rename it, run `git init` to initialize an empty git repository and then get cracking creating your own package.

You will need to update the following items with your package's name and info:

- Rename "composer-package-starter", the main repository directory, to your awesome package's name.
- Edit **/README.md** and add information for your package.
- Edit **/phpunit.xml** and rename `Example Package` to your package's name.
- Edit **/composer.json** (`name`, `description`, `keywords`, `authors`, `autoload.psr-4`, `autoload-dev.psr-4`, etc).
- Edit **/tests/TestCase.php** (rename the database table in `migrateTables()`).
- Edit **/tests/ExampleTest.php** and rename the file for your first test.



## Extras

_The `illuminate/database` package is required for development testing, however if this package is intended to be a Laravel specific package and/or a package that needs database transactions, feel free to move `illuminate/database` from `require-dev` to `require`._
