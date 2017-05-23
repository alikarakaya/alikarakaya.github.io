## Posgresql'de pg_restore yaparken user yetkilendirme. ##
Postgresql'de pg_dump ile almış olduğunuz yedekleri pg_restore ile açmak için 
ilk önce hangi user'ı kullanacağımız belirleyip yada oluşturup daha sonra bu 
user'a  pg_hba.conf dosyasında yetkilendirme yapılması gerekiyor.

```commandline
	# pg_restore -U postgres -Fc backup.bak -d databasename
	```

Eğer pg_hba.conf dosyasında yetkilendirme işleminde postgresql user'ına 

    local   all        postgres            md5



yetkisi verilmemişse yada md5 yerine peer yazıyorsa yetki problemi olacaktır.

