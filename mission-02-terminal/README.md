# Mission 2 — Terminal and File Management

## 1. Task / objective
(What the mission asked you to do in Terminal.)

## 2. Work completed

### Task 2.1 — Basic Terminal operations

| Operation / command name | What it does | What I observed |
|--------------------------|--------------|-----------------|
| Current-directory display (`pwd`) | Shows the full path of the folder I am currently in | /Users/girihimanshu540/Desktop/digital-detective-8036/mission-02-terminal |
| Directory listing (`ls`) | Lists the files and folders in the current location | README.md |
| Detailed listing (`ls -l`) | Lists the same items with extra details like permissions, size and date | -rw-r--r--@ 1 girihimanshu540  staff  2193 Nov 16 01:51 README.md |
| Change directory (`cd`) | Moves me into another folder; `cd ..` moves up to the parent folder | It changed the directory |
| Create directory (`mkdir`) | Creates a new folder | I created a directory named terminal-practice . |
| Create empty file (`touch`) | Creates a new file with nothing inside it | I created a file .  |
| Copy file (`cp`) | Makes a duplicate of a file under a new name, keeping the original | I copied a File . |
| Move / rename file (`mv`) | Renames a file, or moves it to a different place | I moved a file . |
| Display file contents (`cat`) | Prints what is inside a file on the screen | I saw the content inside the file |

### Task 2.2 — Practising file changes

1. Replacing vs adding to the end

"filename" > replaces: it erases whatever the file had and writes the new text in its place.
"filename" >> appends: it keeps the existing content and adds the new text after it.
In your practice, “line one” stayed when you used >> for “line two”, so cat notes.txt showed both lines. If you had used > the second time, only “line two” would be left.

2. Copy vs move

cp makes a duplicate, so you end up with two files: the original and the copy.
mv relocates or renames the file, so you still have the same number of files. The old name or location no longer exists.
Use your own practice as evidence. Count the files with ls after each command.

3. What pwd tells you

It prints the full path from the root of the computer down to the folder you’re in. That tells you exactly where you are in the folder structure, and which folders sit above you.
It’s useful because commands like ls, cp and mkdir act on the current folder, so you can check you’re in the right place before running them.

4. Why ls is useful

It shows you what’s in the current folder: file names, folders, and (with flags) sizes and permissions.
It’s a safe way to check before changing anything, for example to avoid overwriting a file that already has the name you’re about to use, or to confirm a command did what you expected.

### Task 2.3 — Flags and pipes

**Normal listing (`ls`):** README.md                       mission-01-computer-basics      mission-04-programs             mission-07-networking
evidence                        mission-02-terminal             mission-05-numbers-data         mission-08-final-report
mission-00-setup                mission-03-operating-system     mission-06-git-github

**Detailed listing (`ls -lah`):** -rw-r--r--@  1 girihimanshu540  staff   1.6K Nov 16 00:54 README.md
drwxr-xr-x   2 girihimanshu540  staff    64B Nov 16 00:27 evidence
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:30 mission-00-setup
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:30 mission-01-computer-basics
drwxr-xr-x@  4 girihimanshu540  staff   128B Nov 16 01:52 mission-02-terminal
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:31 mission-03-operating-system
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:31 mission-04-programs
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:31 mission-05-numbers-data
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:31 mission-06-git-github
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:31 mission-07-networking
drwxr-xr-x@  3 girihimanshu540  staff    96B Nov 16 00:31 mission-08-final-report

**What each flag changed:**
- `l`: shows each item on its own line with extra details: permissions, owner, size and last-modified date.
- `a`: includes hidden files, which are the ones whose names start with a dot, like .git. It also shows . (the current folder) and .. (the parent folder).
- `h`: shows sizes as 4.0K instead of 4096. It only matters when it’s combined with -l, since that’s where the sizes appear.

**Pipe (`ls -l | head -n 3`):**
- Left side: produces the detailed listing as text.
- Right side: takes that text and keeps only the first 3 lines.
- What `|` does: sends the output of the command on the left into the command on the right as its input, instead of printing it to the screen.

**Observation:** I observed all the things mentioned above .

### Task 2.4 — Package managers

**Commands used:**
- `brew --version`: checks that Homebrew is installed and shows its version
- `brew list`: shows the packages Homebrew has installed

**What I observed:**  Homebrew 7.0.12
                      bison		gettext		libngtcp2	libxml2		msgpack		pkgconf		x264
brotli		git		libpng		lz4		ncurses		qrencode	x265
ca-certificates	groonga		libpsl		lzo		ninja		readline	xz
cmake		json-c		libssh2		m4		onigmo		sdl2-compat	zlib
cowsay		lame		libtool		mariadb		openssl@3	sdl3		zstd
curl		libevent	libunistring	mecab		openssl@4	simdjson
dav1d		libnghttp2	libvmaf		mecab-ipadic	opus		svt-av1
ffmpeg		libnghttp3	libvpx		mpg123		pcre2		telnet


**Why package managers are useful:**
This is used for install many packages at one time in one command .


## 3. Commands / tools used
All the mentioned Command .
