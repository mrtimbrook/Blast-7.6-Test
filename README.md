# Blast + Storybook 7.6

A demo repo to recreate the issues when trying to update blast to use Storybook Server 7.6.12.

## To Install

1. Install deps

```
composer install
```

2. Duplicate `.env.example` and rename to `.env` and update `APP_URL` to `http://127.0.0.1:8000`

3. Start server

```
php artisan serve
```

4. Run blast

```
php artisan blast:launch
```

## Issue

App fails with error when trying to use StoryStoreV7:

```
Error: Error: Unknown node type CallExpression
    at PreviewWeb.getStoryIndexFromServer (http://localhost:6006/sb-preview/runtime.js:87:1192)
```
