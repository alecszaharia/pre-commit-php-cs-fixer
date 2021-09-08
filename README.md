# pre-commit-php-cs
Create a pre-commit hook that will runt the php-cs fixes.

#Configure
1. Add the lib repository in your composer.json
    `repositories: [ 
       {
            "type": "vcs",
            "url": "https://github.com/bagrinsergiu/brizy-texts-extractor.git"
        }
    ]`
2. Run: `composer requre alecszaharia/pre-commit-php-cs`
3. Run: `./bin/install.sh` - this will create a pre-commit hook in .git directory 
4. Create the `php_cs-fixes.dist.php` your project root. The pro-commit hook will fail unless the file exists.
