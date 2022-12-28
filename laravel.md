# Laravel

**Content**
- ORM
  - [How to query between two dates using Laravel and Eloquent](#issue-1)
  - [Update nested json](#issue-2)

<a name="issue-1"></a>
## How to query between two dates using Laravel and Eloquent

```php
 YourModel::query()
    ->where('start', '<=', now()->toDateTimeString())
    ->where('end', '>=', now()->toDateTimeString())
    ->get();
```

read more [stackoverflow](https://stackoverflow.com/a/33361741/19299063)



<a name="issue-2"></a>
## Update nested json
```php
$affected = DB::table('users')
              ->where('id', 1)
              ->update(['options->enabled' => true]);

# note you can use the normal Laravel eloquent (ORM) and it works with updateOrCreate
```
