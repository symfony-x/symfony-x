# PHP-CS-Fixer CLI Cheatsheet

Here's a concise cheatsheet for the **PHP-CS-Fixer CLI**:  

```markdown
# PHP-CS-Fixer CLI Cheatsheet

## Installation
Install via Composer:
```bash
composer require --dev friendsofphp/php-cs-fixer
```

## Fix Code
Fix PHP files in the current directory:
```bash
./vendor/bin/php-cs-fixer fix
```

Fix specific directory or file:
```bash
./vendor/bin/php-cs-fixer fix path/to/file-or-directory
```

## Dry Run (Preview Changes)
Show what would be changed without modifying files:
```bash
./vendor/bin/php-cs-fixer fix --dry-run
```

With verbose output:
```bash
./vendor/bin/php-cs-fixer fix --dry-run -v
```

## Specify Rules
Use predefined rules or a custom ruleset:
```bash
./vendor/bin/php-cs-fixer fix --rules=@PSR12
```

Apply multiple rules:
```bash
./vendor/bin/php-cs-fixer fix --rules="['@PSR12', 'array_syntax' => ['syntax' => 'short']]"
```

## Use Config File
Use a custom `.php-cs-fixer.dist.php` configuration file:
```bash
./vendor/bin/php-cs-fixer fix --config=.php-cs-fixer.dist.php
```

## Cache
Clear the cache:
```bash
./vendor/bin/php-cs-fixer fix --clear-cache
```

Use a custom cache file:
```bash
./vendor/bin/php-cs-fixer fix --cache-file=custom.cache
```

## Lint Mode
Enable linting during fix:
```bash
./vendor/bin/php-cs-fixer fix --allow-risky=yes
```

## Verbosity Levels
Display detailed logs:
```bash
./vendor/bin/php-cs-fixer fix -v
```

Show progress:
```bash
./vendor/bin/php-cs-fixer fix --verbose
```

## Help and Version
Display help information:
```bash
./vendor/bin/php-cs-fixer --help
```

Show current version:
```bash
./vendor/bin/php-cs-fixer --version
```
```

This cheatsheet covers the common commands you'll use with PHP-CS-Fixer for fixing and customizing PHP code formatting in your projects.
