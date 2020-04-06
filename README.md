# after install moodle:
- <strong>feature guide :</strong>
- change favicon
- remove attr footer
- Self registration with no email confirmation
- disable view online user
- assign new admin or creator
- remove forgot password
- noemailever setup

# change favicon
<pre>
$ cd /var/www/moodle #path moodle
$ find ./ -name *.ico
<i>./theme/boost/pix/favicon.ico #you can change this icon
./theme/classic/pix/favicon.ico</i> #you can change this icon
$ chown -R www-data:www-data ./moodle/
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
!!! for registration confirm with admin, download :https://github.com/strongpapazola/moodle_custom_default/raw/master/auth_emailadmin_moodle37_2019072300.zip
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

# assign new admin or creator
<img src="https://github.com/strongpapazola/moodle_custom_default/raw/master/Screenshot%20from%202020-04-06%2013-42-26.png">
<pre>
#just follow the img
</pre>

# remove forgot password
<pre>Edit this file</pre>
<img src="https://github.com/strongpapazola/moodle_custom_default/raw/master/Screenshot%20from%202020-04-06%2018-55-10.png">
<pre>to : </pre>
<img src="https://github.com/strongpapazola/moodle_custom_default/raw/master/Screenshot%20from%202020-04-06%2018-55-47.png">

# noemaileve setup
<pre>edit /<moodle_dir>/config.php</pre>
<img src="https://github.com/strongpapazola/moodle_custom_default/raw/master/Screenshot%20from%202020-04-06%2022-01-11.png"
to : 
<img src="https://github.com/strongpapazola/moodle_custom_default/raw/master/Screenshot%20from%202020-04-06%2022-01-35.png"
