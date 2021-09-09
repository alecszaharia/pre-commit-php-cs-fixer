# pre-commit-php-cs
Create a pre-commit hook that will run the php-cs fixes.

## Configure
1. Add the lib repository in your composer.json
    `repositories: [
      {
      "type": "vcs",
      "url": "https://github.com/alecszaharia/pre-commit-php-cs-fixer.git"
      }
    ]`
2. Run: `composer require alecszaharia/pre-commit-php-cs-fixer`
3. Run: `./vendor/bin/pre-commit-install` - this will create a pre-commit hook in .git directory 
4. Create the `.php_cs-fixes.dist.php` your project root. The pre-commit hook will fail unless the file exists.

WARNING: On Phpstorm make sure that on the commit tool the Run Git Hooks is checked.

## Manual Run
 This will fix all new and modified files.
 Run: `./vendor/bin/run-php-cs-fixer`