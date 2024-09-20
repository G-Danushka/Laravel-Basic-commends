# Laravel Artisan Commands Cheat Sheet
This cheat sheet covers commonly used Laravel Artisan commands for daily development tasks.

## General Commands

- `php artisan serve`  
  Starts the Laravel development server on `http://localhost:8000`.

- `php artisan tinker`  
  Opens an interactive shell to interact with your application.

- `php artisan clear-compiled`  
  Removes the compiled class file.

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

## Database Commands

- `php artisan migrate`  
  Runs all pending migrations.

- `php artisan migrate:rollback`  
  Rolls back the last migration batch.

- `php artisan db:seed`  
  Seeds the database with records using seeders.

- `php artisan migrate:fresh --seed`  
  Drops all tables and re-runs all migrations with seeding.

## Cache Commands

- `php artisan cache:clear`  
  Clears the application cache.

- `php artisan config:cache`  
  Creates a cache file for faster configuration loading.

- `php artisan route:cache`  
  Creates a cache file for faster route registration.

- `php artisan view:clear`  
  Clears all compiled view files.

## Maintenance Commands

- `php artisan down`  
  Puts the application into maintenance mode.

- `php artisan up`  
  Brings the application out of maintenance mode.

## Queue Commands

- `php artisan queue:work`  
  Processes the next job in the queue.

- `php artisan queue:restart`  
  Restarts the queue worker after the current job.

## Route Commands

- `php artisan route:list`  
  Lists all registered routes.

## Test Commands

- `php artisan test`  
  Runs the application tests.

---

Use these commands frequently to streamline your Laravel development workflow.

