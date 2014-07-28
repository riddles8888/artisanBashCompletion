artisanBashCompletion
=====================

This adds bash completion for Laravel 4s artisan CLI.

- Put "listForBash.php" in app/commands/ and register it in app/start/artisan.php with `Artisan::add(new listForBash);`

- Make artisan executable with `chmod +x artisan`

- Create an alias for the php artisan command
`echo 'alias artisan="php artisan"' >> .bash_profile`

- Put the file "artisan" in /etc/bash_completion.d/ and remember to source it with `. /etc/bash_completion.d/artisan` (or source every completion script with `. /etc/bash_completion`) if it does not happen already on your system.
`cp artisan /etc/bash_completion.d/artisan;
source /etc/bash_completion.d/artisan;`

Now use `artisan ` and start tabbing away...

Tested on Debian, Cent OS 6 and php 5.4 (I fancy the new array style, but replace that and it should work with prior versions)

Have fun...

