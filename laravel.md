# Laravel

**Content**
- ORM
  - [How to query between two dates using Laravel and Eloquent](#issue-1)

<a name="issue-1"></a>
## How to query between two dates using Laravel and Eloquent

```php
 YourModel::query()
    ->whereTime('start', '<=', now()->toDateTimeString())
    ->whereTime('end', '>=', now()->toDateTimeString())
    ->get();
```

read more [stackoverflow](https://stackoverflow.com/a/33361741/19299063)
