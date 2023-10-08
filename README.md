# laravel-model-delete
Custom Command to delete laravel models with migrations and database table 

# Usage

**1. Create the Command Class:**

  You can generate a new Artisan command class using the make:command Artisan command. Open your terminal and run the following command, replacing 

    php artisan make:command DeleteModelCommand

  This will create a new command class in the app/Console/Commands directory.

**2. Implement the Command Logic:**

  Open the newly generated command class (located in app/Console/Commands) and copy and paste DeleteModelCommand.php to that file

**3. Register the Command:**

  To make your custom command available, you need to register it in the app/Console/Kernel.php file. Open the Kernel.php file and add your command class to the $commands property's array:

    // app/Console/Kernel.php

    protected $commands = [
        // ...
        \App\Console\Commands\DeleteModelCommand::class,
    ];
    
**4. Run Your Custom Command:**

  You can now run your custom command using Artisan in the terminal:

    php artisan delete:model Demo

  Replace Demo with the actual model name
