```bash
➜  for-umlwriter-discussions-30 git:(master) ✗ composer --version
Composer version 2.8.10 2025-07-10 19:08:33
PHP version 8.3.6 (/usr/bin/php8.3)
```

```bash
➜  for-umlwriter-discussions-30 git:(master) ✗ composer show
myclabs/deep-copy                1.13.4 Create deep copies (clones) of your objects
nikic/php-parser                 5.6.1  A PHP parser written in PHP
phar-io/manifest                 2.0.4  Component for reading phar.io manifest information from a PHP Archive (PHAR)
phar-io/version                  3.2.1  Library for handling version information and constraints
phpunit/php-code-coverage        12.3.2 Library that provides collection, processing, and rendering functionality for PHP code co...
phpunit/php-file-iterator        6.0.0  FilterIterator implementation that filters files based on a list of suffixes.
phpunit/php-invoker              6.0.0  Invoke callables with a timeout
phpunit/php-text-template        5.0.0  Simple template engine.
phpunit/php-timer                8.0.0  Utility class for timing
phpunit/phpunit                  12.3.4 The PHP Unit Testing framework.
psr/container                    2.0.2  Common Container Interface (PHP FIG PSR-11)
sebastian/cli-parser             4.0.0  Library for parsing CLI options
sebastian/comparator             7.1.2  Provides the functionality to compare PHP values for equality
sebastian/complexity             5.0.0  Library for calculating the complexity of PHP code units
sebastian/diff                   7.0.0  Diff implementation
sebastian/environment            8.0.3  Provides functionality to handle HHVM/PHP environments
sebastian/exporter               7.0.0  Provides the functionality to export PHP variables for visualization
sebastian/global-state           8.0.0  Snapshotting of global state
sebastian/lines-of-code          4.0.0  Library for counting the lines of code in PHP source code
sebastian/object-enumerator      7.0.0  Traverses array structures and object graphs to enumerate all referenced objects
sebastian/object-reflector       5.0.0  Allows reflection of object attributes, including inherited and non-public ones
sebastian/recursion-context      7.0.1  Provides functionality to recursively process PHP variables
sebastian/type                   6.0.3  Collection of value objects that represent the types of the PHP type system
sebastian/version                6.0.0  Library that helps with managing the version number of Git-hosted PHP projects
staabm/side-effects-detector     1.0.5  A static analysis tool to detect side effects in PHP code
symfony/console                  5.4.47 Eases the creation of beautiful and testable command line interfaces
symfony/deprecation-contracts    3.6.0  A generic function and convention to trigger deprecation notices
symfony/polyfill-ctype           1.32.0 Symfony polyfill for ctype functions
symfony/polyfill-intl-grapheme   1.32.0 Symfony polyfill for intl's grapheme_* functions
symfony/polyfill-intl-normalizer 1.32.0 Symfony polyfill for intl's Normalizer class and related functions
symfony/polyfill-mbstring        1.32.0 Symfony polyfill for the Mbstring extension
symfony/polyfill-php73           1.32.0 Symfony polyfill backporting some PHP 7.3+ features to lower PHP versions
symfony/polyfill-php80           1.32.0 Symfony polyfill backporting some PHP 8.0+ features to lower PHP versions
symfony/service-contracts        3.6.0  Generic abstractions related to writing services
symfony/string                   6.4.24 Provides an object-oriented API to strings and deals with bytes, UTF-8 code points and gr...
theseer/tokenizer                1.2.3  A small library for converting tokenized PHP source code into XML and potentially other f...
```

```bash
➜  for-umlwriter-discussions-30 git:(master) ✗ php umlwriter-4.3.0.phar --manifest

+-----------------------------------+-----------------------------------+---------------+--------------------------+
| Package                           | Constraint                        | Version       | Dependency's category    |
+-----------------------------------+-----------------------------------+---------------+--------------------------+
| bartlett/umlwriter                |                                   | 4.3.0@4f2903c |                          |
| php                               | requires ^8.2                     |               | Direct (for production)  |
| bamarni/composer-bin-plugin       | requires ^1.8                     | 1.8.2         | Direct (for development) |
| bartlett/graph-plantuml-generator | requires ^1.6                     | 1.6.1         | Direct (for production)  |
| bartlett/graph-uml                | requires ^1.6                     | 1.6.0         | Direct (for production)  |
| cweagans/composer-patches         | requires ^1.7                     | 1.7.3         | Direct (for production)  |
| graphp/graph                      | requires 1.x-dev#0adb04d as 1.0.0 | 1.x-dev       | Direct (for production)  |
| graphp/graphviz                   | requires 1.x-dev#686f747 as 1.0.0 | 1.x-dev       | Direct (for production)  |
| jawira/plantuml                   | requires ^1.2025                  | v1.2025.4     | Direct (for development) |
| jawira/plantuml-encoding          |                                   | v1.1.1        | Transitive               |
| jetbrains/phpstorm-stubs          |                                   | v2024.3       | Transitive               |
| nikic/php-parser                  |                                   | v5.5.0        | Transitive               |
| psr/container                     | requires ^2.0                     | 2.0.2         | Direct (for production)  |
| roave/better-reflection           | requires ^6.0                     | 6.59.0        | Direct (for production)  |
| symfony/config                    | requires ^7.0                     | v7.3.0        | Direct (for production)  |
| symfony/console                   | requires ^7.0                     | v7.3.1        | Direct (for production)  |
| symfony/deprecation-contracts     |                                   | v3.6.0        | Transitive               |
| symfony/filesystem                |                                   | v7.3.0        | Transitive               |
| symfony/finder                    | requires ^7.0                     | v7.3.0        | Direct (for production)  |
| symfony/options-resolver          | requires ^7.0                     | v7.3.0        | Direct (for production)  |
| symfony/polyfill-ctype            |                                   | v1.32.0       | Transitive               |
| symfony/polyfill-intl-grapheme    |                                   | v1.32.0       | Transitive               |
| symfony/polyfill-intl-normalizer  |                                   | v1.32.0       | Transitive               |
| symfony/polyfill-mbstring         |                                   | v1.32.0       | Transitive               |
| symfony/service-contracts         |                                   | v3.6.0        | Transitive               |
| symfony/string                    |                                   | v7.3.0        | Transitive               |
| symfony/yaml                      | requires ^7.0                     | v7.3.1        | Direct (for production)  |
| webmozart/assert                  |                                   | 1.11.0        | Transitive               |
+-----------------------------------+-----------------------------------+---------------+--------------------------+

```

```bash
➜  for-umlwriter-discussions-30 git:(master) ✗ php umlwriter-4.3.0.phar diagram:class --output=. --bootstrap=vendor/autoload.php -- src-php -vvv

Box Requirements Checker
========================

> Using PHP 8.3.6
> PHP is using the following php.ini file:
  /etc/php/8.3/cli/php.ini

> Checking Box requirements:
  ✔ This application requires a PHP version matching "^8.2".
  ✔ The package "symfony/polyfill-mbstring" requires the extension "iconv".
  ✔ The package "nikic/php-parser" requires the extension "json".
  ✔ The package "roave/better-reflection" requires the extension "json".
  ✔ The package "nikic/php-parser" requires the extension "tokenizer".
  ✔ This application requires the extension "zlib".
  ✔ The package "jawira/plantuml-encoding" requires the extension "zlib".
  ✔ The package "symfony/service-contracts" conflicts with the extension "psr".
  
                                                                                                                                      
 [OK] Your system is ready to run the application.                                                                                    
                                                                                                                                      


UML Class Diagram Generation
============================

PHP Fatal error:  Declaration of Symfony\Component\Console\Output\ConsoleSectionOutput::doWrite(string $message, bool $newline) must be compatible with Symfony\Component\Console\Output\StreamOutput::doWrite(string $message, bool $newline): void in /home/np/dev/test/for-umlwriter-discussions-30/vendor/symfony/console/Output/ConsoleSectionOutput.php on line 95

```
