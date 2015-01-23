Dirty Socks!

This depends on having the proper public/private keys set up on your ssh server.

1. Prepare the script. An example is given here in dirty_socks.sh. Move it to the desired directory. In this example, it's in ~/scripts/
2. Prepare the .plist file. Make sure the <string> portion points to the right place.
3. Load the .plist file:
      launchctl load /Users/jasonmorrow/Library/LaunchAgents/com.us_socks.plist 
4. Start the service by hand (it will start on boot hereafter)
      launchctl start com.us_socks
