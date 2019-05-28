1. Setup Mail Server
2. Change User.php or User Model
    //**class User extends Authenticatable implements MustVerifyEmail**//

3. Change web.php
    //**Auth::routes(['verify'=>true]);**//

4. Run Command "php artisan vendor:publish --tag=laravel-notifications"

5. Change HomeController.php
    //** $this->middleware(['auth','verified']); **//

All Set