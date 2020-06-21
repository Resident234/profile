# Мой личный сайт



### Зайти в контейнер 
```
docker exec -it work_resident234_db_1 bash
docker exec -it work_resident234_wordpress_1 bash
cd var/www/html
```

### Раскатать бд 
```
cd var/www/html
mysql -u wordpress -pwordpress wordpress < old_db_with_data.sql
```

### Авиторизоваться под пользоватлем mysql
```
mysql -u wordpress -pwordpress
```

### Экспорт бд
``` 
mysqldump -u wordpress -p wordpress > new_database.sql
```

