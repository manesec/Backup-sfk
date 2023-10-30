# Backup-sfk
 Backup file from Swiss File Knife Files

Version: 1.9.9.0

Backup file from https://sourceforge.net/projects/swissfileknife/files/1-swissfileknife/

# Simple Example 

Example Write by [@manesec](https://github.com/manesec)

## FTP

+ Server: `sfk ftpserv -rw`
+ Client: `sfk ftp <server_ip> put <file>`

## Simple File Transfer

+ Server: `sfk sftserv -rw`
+ Client: `sfk sft 192.168.31.158 put <file>`

More example please goto [here](https://github.com/manesec/maketoolkit-db/blob/main/MKTTools/Tools/SFK.md).

# Full command

```cmd
C:\Users\Mane\Downloads>sfk198.exe
SFK - The Swiss File Knife Multi Function Tool.
Release 1.9.8 Base/XD Revision 2 of Sep 20 2022.
StahlWorks Technologies, http://stahlworks.com/
Distributed for free under the BSD License, without any warranty.

type "sfk commandname" for help on any of the following.
some commands require to add "-help" for the help text.

   file system
      sfk list       - list directory tree contents.
                       list latest, oldest or biggest files.
                       list directory differences.
                       list zip jar tar gz bz2 contents.
      sfk olist      - list office files in a folder,
                       like .docx .xlsx .ods .odt
      sfk filefind   - find files by filename
      sfk treesize   - show directory size statistics
      sfk copy       - copy directory trees additively
      sfk sync       - mirror tree content with deletion
      sfk rename     - flexible multi file rename
      sfk partcopy   - copy part from a file into another one
      sfk mkdir      - create directory tree
      sfk delete     - delete files and folders
      sfk deltree    - delete whole directory tree
      sfk deblank    - remove blanks in filenames
      sfk space [-h] - tell total and free size of volume
      sfk filetime   - tell times of a file
      sfk touch      - change times of a file
      sfk index      - create index file(s) for fast lookup
      sfk name       - lookup file names using index files
      sfk fixfile    - change bad filenames and file times
      sfk setbytes   - set bytes at offset within a file

   compression
      sfk zip        - create zip file from folder
      sfk zipto      - zip selected file list
      sfk unzip      - list or extract zip file
      sfk checkzip   - verify zip file content

   conversion
      sfk oload      - load office file content as text
      sfk lf-to-crlf - convert from LF to CRLF line endings
      sfk crlf-to-lf - convert from CRLF to LF line endings
      sfk detab      - convert TAB characters to spaces
      sfk entab      - convert groups of spaces to TAB chars
      sfk scantab    - list files containing TAB characters
      sfk split      - split large files into smaller ones
      sfk join       - join small files into a large one
      sfk csvtotab   - convert .csv data to tab separated
      sfk tabtocsv   - convert tab separated to .csv format
      sfk encode     - convert data to base64 or hex format
      sfk decode     - decode base64, hex or url format
      sfk wtoa       - convert wide chars to Ansi
      sfk wtou       - convert wide chars to UTF-8
      sfk utoa       - convert UTF-8 text to Ansi
      sfk hexdump    - create hexdump from a binary file
      sfk hextobin   - convert hex data to binary
      sfk hex        - convert decimal number(s) to hex
      sfk dec        - convert hex number(s) to decimal
      sfk chars      - print chars for a list of codes
      sfk bin-to-src - convert binary to source code
      sfk uuencode   - encode binary files as plain text

   text processing
      sfk filter     - search, filter and replace text data
      sfk ofilter    - filter  text from an office file
      sfk replace    - replace words in binary and text files
      sfk xed        - edit stream text using sfk expressions
      sfk xex        - extract from stream text using expressions
      sfk xreplace   - Plus/XE: replace in files using expressions
      sfk run        - run external command on all files of a folder
      sfk runloop    - run a command n times in a loop
      sfk printloop  - print some text many times
      sfk load       - load file content for further processing
      sfk perline    - run sfk command(s) per input text line
      sfk head       - print first lines of a file
      sfk tail       - print last lines of a file
      sfk snapto     - join many text files into one file
      sfk addhead    - insert string at start of text lines
      sfk addtail    - append string at end of text lines
      sfk joinlines  - join text lines split by email reformatting
      sfk strings    - extract strings from a binary file
      sfk sort       - sort text lines produced by another command
      sfk count      - count text lines, filter identical lines
      sfk difflines  - show text lines differing between files
      sfk linelen    - tell length of string(s)

   search and compare
      sfk xfind      - search in text files using
                       wildcards and simple expressions
      sfk ofind      - search in office files .docx .xlsx .ods
      sfk xfindbin   - search in text and binary files
      sfk xhexfind   - search with hexdump output
      sfk extract    - extract data from text and binary
      sfk find       - search static text, without wildcards
      sfk hexfind    - search static binary data
      sfk md5gento   - create list of md5 checksums over files
      sfk md5check   - verify list of md5 checksums over files
      sfk md5        - calc md5 over a file, compare two files
      sfk pathfind   - search PATH for location of a command
      sfk reflist    - list fuzzy references between files
      sfk deplist    - list fuzzy dependencies between files
      sfk dupfind    - find duplicate files by content

   networking
      sfk httpserv   - run an instant HTTP server.
                       type "sfk httpserv -help" for help.
      sfk ftpserv    - run an instant FTP server
                       type "sfk ftpserv -help" for help.
      sfk ftp        - instant FTP client
      sfk web        - send HTTP request to a server
      sfk wget       - download HTTP file from the web
      sfk tcpdump    - print TCP conversation between programs
      sfk udpdump    - print incoming UDP requests
      sfk udpsend    - send UDP requests
      sfk ip         - tell own machine's IP address(es).
                       type "sfk ip -help" for help.
      sfk netlog     - send text outputs to network,
                       and/or file, and/or terminal
      sfk fromnet -h - receive and print network text
      sfk ping       - ping multiple machines in one go
      sfk pingdiff   - find ip of new devices

   scripting
      sfk help chain - how to combine multiple commands
      sfk batch      - run many sfk commands in a script file
      sfk label      - define starting points within a script
      sfk call       - call a sub function at a label
      sfk echo       - print (coloured) text to terminal
      sfk color      - change text color of terminal
      sfk setvar     - put text into an sfk variable
      sfk storetext  - store text in memory for later use
      sfk alias      - create command from other commands
      sfk mkcd       - create command to reenter directory
      sfk sleep      - delay execution for milliseconds
      sfk pause      - wait for user input
      sfk stop       - stop sfk script execution
      sfk tee        - split command output in two streams
      sfk tofile     - save command output to a file
      sfk toterm     - flush command output to terminal
      sfk for        - repeat commands many times
      sfk loop       - repeat execution of all commands
      sfk cd         - change directory within a script
      sfk getcwd     - print the current working directory
      sfk require    - compare version text
      sfk time [-h]  - print current date and time

   development
      sfk bin-to-src - convert binary data to source code
      sfk make-random-file - create file with random data
      sfk fuzz       - change file at random, for testing
      sfk sample     - print example code for programming
      sfk patch      - change text files through a script
      sfk inst       - instrument c++ with tracing calls

   diverse
      sfk view       - show text output in a GUI tool,
                       for interactive browse and filter
      sfk status     - send colored status to the SFKTray
                       Windows GUI utility for display
      sfk calc       - do a simple instant calculation
      sfk random     - create a random number
      sfk prompt     - ask for user input
      sfk number     - print number in diverse formats
      sfk xmlform    - reformat xml  for easy viewing
      sfk jsonform   - reformat json for easy viewing
      sfk video      - how to edit video files
      sfk toclip     - copy command output to clipboard
      sfk fromclip   - read text from clipboard
      sfk env        - search environment variables
      sfk version    - show version of a binary file
      sfk ascii      - list Ansi codepage characters
      sfk ascii -dos - list OEM  codepage characters
      sfk spell      - phonetic spelling for telephone
      sfk cmd        - print an example command
      sfk ruler      - measure console text width
      sfk license    - print the SFK license text
      sfk update     - check for SFK updates
      sfk data       - create random text and test data

   help by subject
      sfk help office   - how to search in office files
      sfk help select   - how dirs and files are selected in sfk
      sfk help options  - general options reference
      sfk help patterns - wildcards and text patterns within sfk
      sfk help chain    - how to combine (chain) multiple commands
      sfk help var      - how to use sfk variables and parameters
      sfk samp          - example scripts on sfk use and for
                          http web access automation
      sfk help shell    - how to optimize the windows command prompt
      sfk help chars    - about locale specific characters
      sfk help nocase   - about case insensitive search
      sfk help unicode  - about unicode file reading support
      sfk help colors   - how to change result colors
      sfk help compile  - how to compile sfk on any linux system

   first time user?

      type "sfk basic" for very basic informations about
      how to select files, general options, shell preparation,
      complex <>|!&?* character issues and color setup.

   to search ALL help text for a topic:

      type "sfk ask word1"    to search all for word1.
      type "sfk ask w1 w2"    to search all for w1 or w2.
      type "sfk dumphelp"     to print ALL help text.

   +----------------------------------------------------------+
   |               Useful? Buy a new coffee mug!              |
   |                   stahlworks.com/merch                   |
   |----------------------------------------------------------|
   |       Get these addons to boost your daily work:         |
   |----------------------------------------------------------|
   |  SFK E-Book : A PDF optimized for your smart phone.      |
   |  SFK Plus   : Fast (x)replace, HTTPS web access and      |
   |               27 status lights in the system tray.       |
   |  DView Pro  : Search 10,000 text files per second.       |
   |               Fly over 100,000 files in one window.      |
   |----------------------------------------------------------|
   |             Read more on www.stahlworks.com              |
   +----------------------------------------------------------+
```