Redirect for YunoHost 
----------------------------------------
Warning: This YunoHost app is still in development. Use it at your own risk!

This app allows to redirect one port and/or path in order to add it as a Yunohost app.
For example, you can create a YunoHost application "MyApp" at "http://domain.tld/myapp" which is actually pointing at "http://127.0.0.1:8080/app". You can even add SSO to protect this application (but make sure that this application CANNOT be accessed by its port).

The main use of redirect_ynh is to create YunoHost apps out of Docker containers: https://github.com/scith/docker_container_ynh. For example, a container running with the option "-p 127.0.0.1:8080:80" could be redirected to "http://domain.tld/myapp" with SSO.

IMPORTANT: the redirect.conf file might need to be updated according to your situation! 

