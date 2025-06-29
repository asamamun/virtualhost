# virtualhost
 <h3>Host file path : C:\Windows\System32\drivers\etc\hosts</h3>
<code>
 <pre>
127.0.0.1   localhost
127.0.0.1   server.test
127.0.0.1   socialapp.test
</pre>
 </code>

<h3>httpd-vhosts.conf file path : C:\xampp8\apache\conf\extra\httpd-vhosts.conf</h3>

<code>
 <pre>
<VirtualHost *:80>
    ServerName localhost
    DocumentRoot "D:/xampp8240/htdocs/"
    <Directory "D:/xampp8240/htdocs/">
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>

# server.dev
<VirtualHost *:80>
    ServerName server.test    
    DocumentRoot "D:/xampp8240/htdocs/ROUND64/"
    <Directory "D:/xampp8240/htdocs/ROUND64/">
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>

# socialapp.test
<VirtualHost *:80>
    ServerName socialapp.test
    DocumentRoot "D:/xampp8240/htdocs/ROUND64/PHP/social-talk/"
    <Directory "D:/xampp8240/htdocs/ROUND64/PHP/social-talk/">
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
</pre>
 </code>
 <hr>
 <h3>Uncomment in httpd.conf</h3>
 <code>
  <pre>
   # Virtual hosts
   Include conf/extra/httpd-vhosts.conf
  </pre>
 </code>
 <hr>
 <p>Now you can visit localhost, server.test and socialapp.test links in browser</p>
