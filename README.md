# after install moodle:
- <strong>feature guide :</strong>
- change favicon
- remove attr footer
- Self registration with no email confirmation
- disable view online user

# change favicon
<pre>
$ cd /var/www/moodle #path moodle
$ find ./ -name *.ico
<i>./theme/boost/pix/favicon.ico #you can change this icon
./theme/classic/pix/favicon.ico</i> #you can change this icon
$ chown -R www-data:www-data /var/www/moodle/
</pre>

# remove attr footer
<pre>
$ nano ./theme/boost/templates/footer.mustache
#edit with your heart
</pre>

# Self registration with no email confirmation
<pre>
$ chown -R www-data:www-data /var/www/moodle/ #make moodle writable plugin
#download onlineconfirm.zip : https://github.com/strongpapazola/moodle_custom_default/raw/master/onlineconfirm.zip
#go to your moodle, Site administration -> plugin -> install plugin
#drag plugin after downloaded and install
#then setup self reg on : administration -> plugin -> Authentication -> Manage authentication
 - disable Email-based self-registration
 - enable Online Confirm
#save
</pre>

# disable view online user
<pre>
#go to Site Admin > Plugins > Blocks > Manage Blocks and hide it there.
</pre>
