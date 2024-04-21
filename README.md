# Laravel Initial Setup

## Prepare Environment

### For Windows

#### 1. Prepare php

1. Download and Install [XAMPP](https://www.apachefriends.org/download.html)
2. Add XAMPP/php to PATH
3. Open a terminal and then type command below to verify php is installed and added to PATH

   ```
   php --version
   ```

#### 2. Prepare composer

1. Download and Install [Composer](https://getcomposer.org/download/)
2. Make sure to Add to PATH when asked
3. Open a terminal and then type command below to verify composer is installed and added to PATH

   ```
   composer --version
   ```

#### 3. Prepare node and npm

1. Download and install [nvm for windows](https://github.com/coreybutler/nvm-windows/releases). Pick the latest nvm-setup.exe
2. Make sure to Add to PATH when asked
3. Open a terminal and then type this command to install latest Node LTS

   ```
   nvm install lts
   nvm use lts
   ```

4. Make sure to node and npm is installed

   ```
   node --version
   npm --version
   ```

## Initialize Laravel Project

### Create a Laravel Project

1. Use this command to create the project, replace example-app with your project name

   ```
   composer create-project laravel/laravel example-app
   ```

2. Run this command to serve laravel project
   ```
   php artisan serve
   ```

### Install Laravel Breeze for Auth Scaffolding

1. Install Laravel Breeze, you can choose the stack of your preference. Up to you which stack: Blade template for the frontend, or Inertia with React/Vue or you can also choose Livewire

   ```
   php artisan breeze:install
   ```

2. Run migration

   ```
   php artisan migrate
   ```

3. Install node dependecies (for Inertia with React or Vue)

   ```
   npm install
   ```

4. Compile frontend assests

   ```
   npm run dev
   ```
