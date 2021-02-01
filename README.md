# laravel-real-time-notifications
# php artisan serve
# php artisan websockets:serve
# php artisan tinker
#public channel
event(new App\Events\RealTimeMessage('Hello World'));
#private channel
event(new App\Events\RealTimeMessagePrivate('Hello World'));
#private noti
$user = User::first();
$user->notify(new App\Notifications\RealTimeNotification('Hello World'));
