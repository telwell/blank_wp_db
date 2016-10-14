# Fresh WordPress DB

I needed to grab the SQL dump of a vanilla WordPress DB installation (for taking a site from a multisite to a stand-alone WordPress site). Unfortunately, I couldn't easily find a fresh WP database installation. Here's one that will hopefully make your life a little easier if you need it as well. 

# Why wp_users & wp_usermeta?

When transfering site files from a Multisite, I avoid bringing in the wp_users and wp_usermeta DBs from the Multisite as they have **every** user for the entire multisite. Rather, using this SQL it will initialize with a user with username **admin** and password **password** . 

You should be able to change that in the SQL yourself or in the WP settings once you're installed.
