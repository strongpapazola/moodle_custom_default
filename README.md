# after install moodle:
- <strong>feature guide :</strong>
- change favicon
- remove attr footer
- self-registration
- disable view online user

# change favicon
<pre>
$ `find ./ -name *.ico`
<i>./theme/boost/pix/favicon.ico
./theme/classic/pix/favicon.ico</i>
$ `chown -R www-data:www-data /var/www/moodle/`
</pre>
