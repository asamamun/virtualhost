# virtualhost
 <h3>Host file path : C:\Windows\System32\drivers\etc\hosts</h3>
<code>
127.0.0.1   localhost
127.0.0.1   myapp.test
127.0.0.1   quizapp.test

<h3>httpd-vhosts.conf file path : C:\xampp8\apache\conf\extra\httpd-vhosts.conf</h3>

<code>
 <pre>
<VirtualHost *:80>
ServerName localhost
DocumentRoot "C:/xampp8/htdocs/"
</VirtualHost>

<VirtualHost *:80>
    ServerName myapp.test
    ServerAlias myapp.local
    DocumentRoot "C:/xampp8/htdocs/r49/react/snactum/test-app/public"
</VirtualHost>
<VirtualHost *:80>
    ServerName quizapp.test
    DocumentRoot "C:/xampp8/htdocs/r49/laravel/projects/TigerQuiz/public"
</VirtualHost>
</pre>
 </code>
