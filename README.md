# get-stuff-done

get-stuff-done is an easy to use command line program that blocks websites known to distract us from our work.

After cloning this repository, put it in your $PATH and ensure it is executable.

Execute it as root because it modifies your hosts file and restarts your network daemon.

## To get-stuff-done

    $ sudo get-stuff-done work

## To no longer get-stuff-done

    $ sudo get-stuff-done play

### $siteList

Add or remove elements of this array for sites to block or unblock.

### ~/.get-stuff-done.ini

Appends additional sites to block.  Duplicates will be removed, and www is prepended.

    sites = foo.com, bar.com, baz.com

### $restartNetworkingCommand

Update this variable with the path to your network daemon along with any parameters needed to restart it.

### $hostsFile

Update this variable to point to the location of your hosts file. Make sure it is an absolute path.

