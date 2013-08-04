lirc-python
===========

Python wrapper for LIRC calls, based on https://github.com/slimjim777/web-irsend

## Usage

Here are some example calls:

    >>> from lirc import Lirc
    >>> lirc_obj = Lirc()

    # Show hooked up devices:
    >>> print ", ".join(lirc_obj.devices())
    zenith
    
    # Send a command
    >>> lirc_obj.send_once('zenith', 'KEY_POWER')
