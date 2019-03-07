In case you get this issue ` dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem.`

And even if you run `sudo dpkg --configure -a` it hangs on installation try the following:
- `sudo rm /var/lib/apt/lists/lock`
- `sudo rm /var/cache/apt/archives/lock`
- `sudo rm /var/lib/dpkg/lock`
- `sudo dpkg --configure -a`

This should only be used as a last resort.
