What's it for
=============

Sometimes in a shell you want to do this:

    echo 'My line ' >> /etc/some_root_only_file

to a file, but it won't work. Instead, this will work:

    sudo sh -c 'echo "My line" >> /etc/some_root_only_file'

but it is painful to type and easy to make error.

`suwrite` is an attempt to fix this. It lets you do

    echo 'My line' |suwrite -a /etc/some_root_only_file

No nested quotes. Tab completion works well.

Usage
=====
    $ suwrite -h
    Usage: suwrite <options> file1 file2 file3
    Options:
    	-a, --append: Append to files instead of overwriting
    	-f, --force: Force overwriting existing files
    