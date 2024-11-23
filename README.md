# Laravel Artisan Commands Cheat Sheet
This cheat sheet covers commonly used Laravel Artisan commands for daily development tasks.

## Installation and Setup Commands

- `composer create-project laravel/laravel project-name`
  Using Composer: Installs a new Laravel application.

- `laravel new project-name`
  Using Laravel Installer: Creates a new Laravel project if the Laravel Installer is globally installed.

- `composer install`
  Installs project dependencies specified in the composer.json file.

## General Commands

- `php artisan key:generate`
  Generates a new application key in the .env file.

- `php artisan serve`  
  Starts the Laravel development server on `http://localhost:8000`.

- `php artisan tinker`  
  Opens an interactive shell to interact with your application.

- `php artisan clear-compiled`  
  Removes the compiled class file.

- `php artisan inspire`
  Displays an inspiring quote.

- `php artisan list`
  Lists all available Artisan commands.

- `php artisan help CommandName`
  Displays help for a specific Artisan command.

## Make Commands

- `php artisan make:controller ControllerName`  
  Used to create a new controller.

- `php artisan make:controller ControllerName --resource`  
  Creates a new resource controller with RESTful methods.

- `php artisan make:model ModelName`  
  Creates a new Eloquent model.

- `php artisan make:model ModelName -m`  
  Creates a new Eloquent model with a migration file.

- `php artisan make:migration create_table_name_table`  
  Creates a new migration file.

- `php artisan make:seeder SeederName`  
  Creates a new database seeder.

- `php artisan make:factory FactoryName`  
  Creates a new factory for generating fake data.

- `php artisan make:middleware MiddlewareName`  
  Creates a new middleware class.

- `php artisan make:request RequestName`  
  Creates a new form request validation class.

- `php artisan make:job JobName`  
  Creates a new job class.

- `php artisan make:event EventName`  
  Creates a new event class.

- `php artisan make:listener ListenerName`  
  Creates a new listener class for handling events.

- `php artisan make:command CommandName`  
  Creates a new Artisan command.

- `php artisan make:policy PolicyName`  
  Creates a new policy class for authorization.

- `php artisan make:notification NotificationName`
  Creates a new notification class.

- `php artisan make:mail MailClassName`
  Creates a new mailable class for sending emails.

- `php artisan make:test TestName`
  Creates a new test class (unit or feature test).

- `php artisan make:rule RuleName`
  Creates a new validation rule class.

## Database Commands

- `php artisan migrate`  
  Runs all pending migrations.

- `php artisan migrate:rollback`  
  Rolls back the last migration batch.

- `php artisan db:seed`  
  Seeds the database with records using seeders.

- `php artisan migrate:fresh --seed`  
  Drops all tables and re-runs all migrations with seeding.

- `php artisan migrate:status`
  Displays the status of each migration.

- `php artisan schema:dump`
  Dumps the current database schema and migrations into a schema file.

## Cache Commands

- `php artisan cache:clear`  
  Clears the application cache.

- `php artisan config:cache`  
  Creates a cache file for faster configuration loading.

- `php artisan route:cache`  
  Creates a cache file for faster route registration.

- `php artisan view:clear`  
  Clears all compiled view files.

- `php artisan event:clear`
  Clears all cached events and listeners.

- `php artisan event:cache`
  Creates a cache file for events and listeners.

## Maintenance Commands

- `php artisan down`  
  Puts the application into maintenance mode.

- `php artisan up`  
  Brings the application out of maintenance mode.

- `php artisan down --secret="secret-key"`
  Allows access to the application in maintenance mode using a secret key.

- `php artisan down --render="errors::503"`
  Specifies a custom view to display in maintenance mode.

## Queue Commands

- `php artisan queue:work`  
  Processes the next job in the queue.

- `php artisan queue:restart`  
  Restarts the queue worker after the current job.

- `php artisan queue:listen`
  Continuously listens to the queue for new jobs.

- `php artisan queue:failed`
  Lists all failed queue jobs.

- `php artisan queue:retry JobID`
  Retries a failed job using its ID.

- `php artisan queue:flush`
  Flushes all failed queue jobs.

## Route Commands

- `php artisan route:list`  
  Lists all registered routes.

- `php artisan route:clear`
  Clears the route cache.

## Test Commands

- `php artisan test`  
  Runs the application tests.

- `php artisan test --filter=TestName`
  Runs a specific test class or method.

## Additional Setup Commands

- `composer require laravel/breeze --dev`
- `php artisan breeze:install`
- `npm install && npm run dev`
  Installs Laravel Breeze for authentication scaffolding.

- `composer require laravel/ui`
- `php artisan ui bootstrap --auth`
- `npm install && npm run dev`
  Installs traditional Bootstrap-based authentication views.

- `php artisan schedule:run`
  Runs scheduled tasks defined in the schedule() method of the App\Console\Kernel class.

## Additional Useful Commands

- `php artisan storage:link`
  Creates a symbolic link to the storage directory for public access.
  public/storage to storage/app/public.

- `php artisan auth:clear-resets`
  Clears expired password reset tokens.

- `php artisan optimize`
  Optimizes the application for better performance.

- `php artisan optimize:clear`
  Clears all cached files (config, route, view, etc.).

- `php artisan package:discover`
  Rebuilds the package cache.

---

Use these commands frequently to streamline your Laravel development workflow.

