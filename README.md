# Creating Navbar file and Call in Index.php

- We will use multiple headers, therefore we move all headers in one folder `header`. And the we used `get_template_part()`.
- If there is only one header file then there is no need to separate folder. In this case, we will create `header.php` in root directory and use `get_header()`.

## Version 1 (v1)

- Create navbar-header.php in `v1/header` folder
- The `navbar-header.php` contains `<header>` tag and `navbar-header` CSS-class. On base of these two things, we will further style it in `functions.php`.
- Code for navbar-header.php is given below

```ruby
<nav class="nav-header" style="display: flex; justify-content: space-between;">
    <div><a href="#">Home</a></div>
    <div><a href="#">About</a></div>
    <div><a href="#">Contact</a></div>
    <div><a href="#">Services</a></div>
</nav>
```

- The `index.php` file will call navbar-header.php` file by using follwoing line.

```ruby
<?php get_template_part('header/navbar-header'); ?>
```
