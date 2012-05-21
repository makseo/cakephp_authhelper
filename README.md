Cakephp Auth Helper
==================

I have often asked how to check is user authorized or not, or how to get e-mail or other authorization data.
For this purpose, I developed this simple helper.

just copy AuthHelper.php to your app/View/helpers folder and add this code to your controller

```php
public $helpers = array('Auth');
```

After that you can use it in your views such as in controllers

Example

```php
<?php $this->Auth->loggedIn(): ?>
<b>Welcome, <?php echo $this->Auth->get('username'); ?>!</b>
<?php endif; ?>
```