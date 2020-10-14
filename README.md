This is a slightly modified version of pyperclip 1.8.1 fixing an attribution error, renamed to pyp3rclip as this may break python 2 compatibility.

The description below is from the original pyperclip repository: https://github.com/asweigart/pyperclip

Pyp3rclip is a cross-platform Python module for copy and paste clipboard functions. It works with Python 2 and 3.

Install on Windows: `pip install pyp3rclip`

Install on Linux/macOS: `pip3 install pyp3rclip`

Al Sweigart al@inventwithpython.com
BSD License

Example Usage
=============

    >>> import pyp3rclip
    >>> pyp3rclip.copy('The text to be copied to the clipboard.')
    >>> pyp3rclip.paste()
    'The text to be copied to the clipboard.'


Currently only handles plaintext.

On Windows, no additional modules are needed.

On Mac, this module makes use of the pbcopy and pbpaste commands, which should come with the os.

On Linux, this module makes use of the xclip or xsel commands, which should come with the os. Otherwise run "sudo apt-get install xclip" or "sudo apt-get install xsel" (Note: xsel does not always seem to work.)

Otherwise on Linux, you will need the gtk or PyQt4 modules installed.
