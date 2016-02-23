# Apache Configuration
```apache
<VirtualHost *:80>
    ServerName  @server_name
    DocumentRoot @document_root

    <Directory @document_root>
        Order allow,deny
        Allow from all
        Require all granted
    </Directory>

    ErrorLog @document_root/error.log
    CustomLog @document_root/access.log combined
</VirtualHost>
```
