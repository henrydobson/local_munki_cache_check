# OSX_LocalMunkiCache

Place this into `/usr/local/munki/preflight.d/`. 
The script checks for local repositories by checking DNS for `munki-cache` then `munki`. 
If a local cache is onsite then the DNS record should be `munki-cache` or `munki`. 
The script fails over to the SoftwareRepoURL stored in the `/Library/Preferences/ManagedInstalls.plist`.
