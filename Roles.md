Доступи до модулів надаються в профілях. Ієрархія наступна: кожен
**користувач** належить до певної **ролі**. Політика доступу кожної ролі визначена її **профілем**.

Тобто: профіль -> роль -> користувач

Керування цим функціоналом знаходиться в адмінській частині в вкладці **Дозволи**. 


customs=# UPDATE "Users" SET email='operator' WHERE username='operator';
UPDATE 1
customs=# UPDATE "Users" SET password='$2b$10$DWqo839PMFJucVA2VPdED.M6xWW1CgBUrVgm6KAyxclNuWyh5G7RW' WHERE username='operator';
