command find:

Option 1: -name

The -name option allows you to search for files based on their names.

Example 1:

<pre><code>

$ find ./written_2 -name "*.txt"
./written_2/notes/notes.txt
./written_2/files/file1.txt
./written_2/files/file2.txt
./written_2/files/file3.txt

</code></pre>

This command searches the ./written_2 directory and its subdirectories for files that end with .txt. The output shows the names of the 4 .txt files that were found.

Example 2:

<pre><code>
$ find ./written_2 -name "notes*"
./written_2/notes
./written_2/notes/notes.txt
</code></pre>

This command searches the ./written_2 directory and its subdirectories for files that have the word "notes" at the beginning of their names. The output shows the name of the directory notes and the file notes.txt inside it.


Option 2: -type

The -type option allows you to search for files based on their type (e.g., regular file, directory, symbolic link, etc.).

Example 1:
<pre><code>
$ find ./written_2 -type f
./written_2/notes/notes.txt
./written_2/files/file1.txt
./written_2/files/file2.txt
./written_2/files/file3.txt
</code></pre>

This command searches the ./written_2 directory and its subdirectories for regular files. The output shows the names of the 4 regular files that were found.

Example 2:
<pre><code>
$ find ./written_2 -type d
./written_2/notes
./written_2/files
</code></pre>

This command searches the ./written_2 directory and its subdirectories for directories. The output shows the names of the 2 directories that were found.

Source: https://manpages.ubuntu.com/manpages/trusty/man1/find.1.html

Option 3: -size

The -size option allows you to search for files based on their size.

Example 1:
<pre><code>
$ find ./written_2 -size +100k
./written_2/notes/notes.txt

</code></pre>

This command searches the ./written_2 directory and its subdirectories for files that are larger than 100 kilobytes.
The output shows the name of the file notes.txt that was found.

Example 2:
<pre><code>
$ find ./written_2 -size -10k
./written_2/files/file1.txt
./written_2/files/file2.txt
./written_2/files/file3.txt

</code></pre>

This command searches the ./written_2 directory and its subdirectories for files that are smaller than 10 kilobytes.
The output shows the names of the 3 files file1.txt, file2.txt, and file3.txt that were found.

(Some resourses and ideas provided by the ChatGpt with links: Source: (https://manpages.ubuntu.com/manpages/trusty/man1/find.1.html ) Source: (https://manpages.ubuntu.com/manpages/trusty/man1/find.1.html)

