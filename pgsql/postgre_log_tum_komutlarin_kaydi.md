Postgres'de tüm CRUD işlemlerinin loglarını kayıtaltına almak için
postgresql.conf dosyasında aşagıdaki satırdaki değişikliği yapmak gerekir.


log_statment = 'all'

Eger sadece UPDATE ve INSERT komutları için

log_statment = 'mod'


