### desc
now can't write the right code, below code is just example.
### dao
```
return errors.Wrapf(errors.NotFound, fmt.Sprintf("sql: %s error: %v", sql, err))
```
### biz
```
if errors.Is(err, errors.NotFound) {}
```
```
if errors.Reason(err, xxxx) == xxxx {}
```