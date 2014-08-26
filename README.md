# Archive
Archive - tool for those who works with many popular archive formats (rar, zip and tar) a lot and want to avoid using different tools from command line.

# Installation
## Linux
If you want install that program for current directory only:
```
wget -O archive https://github.com/wapmorgan/archive/raw/master/archive.php && chmod +x archive
```

If you want install that program for all system (run as root):
```
wget -O archive https://github.com/wapmorgan/archive/raw/master/archive.php && chmod +x archive
mv archive /usr/local/bin
```

## Windows


# Usage
Usage is pretty simple:
    `archive [archive] {action} FILES... [--listFormat=] [--extractDir=]`
ACTIONS
  **index**
   You can get the list of files stored in archive. By passing `--listFormat`
    option you can specify output format. It has syntax similar to sprintf()
    format. The main improvement is you can specify placeholders like this:
    @placeholder%format where placeholder is an identificator of property for
    array entry. Standart listFormat: '@name%40s | @size%d | @time%s'.
  **extract**
   Extract archive files to dir. By passing `--extractDir` option you can
    specify output directory.
  **print FILES...**
   Print the files contents to standard output. Useful for on-the-fly
    searching.

Run `archive` without arguments to see all manual.
