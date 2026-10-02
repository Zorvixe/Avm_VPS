```bash
CREATE USER avmuser WITH ENCRYPTED PASSWORD 'avmpassword';
```
```bash
CREATE DATABASE avmdb OWNER avmuser;
```
```bash
GRANT ALL PRIVILEGES ON DATABASE avmdb TO avmuser;
```
```bash
DATABASE_URL=postgresql://avmuser:avmpassword@127.0.0.1:5432/avmdb
```

```bash
 nano /etc/nginx/sites-available/avmagrilifescience.com.conf
```
```bash
 nano /etc/nginx/sites-available/app.avmagrilifescience.com.conf
```
```bash
nano /etc/nginx/sites-available/api.avmagrilifescience.com.conf
```

```bash
ln -s /etc/nginx/sites-available/avmagrilifescience.com.conf /etc/nginx/sites-enabled/
```
```bash
ln -s /etc/nginx/sites-available/app.avmagrilifescience.com.conf /etc/nginx/sites-enabled/
```
```bash
ln -s /etc/nginx/sites-available/api.avmagrilifescience.com.conf /etc/nginx/sites-enabled/
```


