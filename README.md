# Before Installing Laravel Project Please check

1. Xampp Install
2. C:\xampp\php\php.ini remove ->';'extension=zip
3. Composer Install
4. node.js must Install
5. Any Code Editor

# Now install Laravel using

> Press Shift+RightClick on htdocs folder
> Open with powershell or any terminal

`composer create-project laravel/laravel Anyname-app`

## Awesome! Laravel is Installed

### What Now??

> Important Folder to know:
1. app>Http>>Controllers,Middleware
2. database>migration
3. resources>views>>index.html file
4. route>create URL
5. public>All css & Javascript

# How to run Laravel Server:

> Press Shift+RightClick on htdocs\Anyname-app folder
> Open with powershell or any terminal

`php artisan serve`

# To know All command:

`php artisan`

# How to create login & registration:

1.Go to [Breeze](https://laravel.com/docs/10.x/starter-kits)

>copy & paste

`composer require laravel/breeze --dev`

`php artisan breeze:install`


# Before migration you need:
1. Go to [Database](localhost/phpmyadmin)
2. create a new database with Anyname-app
3. open Laravel Project with code Editor
4. Open .env file
5. change DB_DATABASE=laravel <- database name you created just Now
6. run bellow command

`php artisan migrate`
`npm install`
`npm run dev`

7. If design breaks then

`npm run build`
`npm run dev`

# How To create Controllers in Laravel:
1. run this command
2. The name of controller here --WebsiteController you can provide anyName
` php artisan make:controller WebsiteController`

3. Go to Http>controller>>WebsiteController Openfile

`class WebsiteController extends Controller{
    `public function __construct(){`
      `  $this->middleware('auth'); // <-- Jodi login sara dukhte na deya hoy
    `}`

      `public function index(){`
      `echo "Welcome MO Rakib!";`
    `}`
`}`

# How to make route:
1. Openfile route>web.php
2. Go To [Routing](https://laravel.com/docs/10.x/routing)
3. copy&paste this:
`use App\Http\Controllers\WebsiteController;`
`Route::get('anyName', [WebsiteController::class, 'index']);`