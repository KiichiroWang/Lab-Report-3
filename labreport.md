# Lab Report 3

### The `find` Command













1. **-type**

*find -type f*
```
$ find -type f
./911report/chapter-1.txt
./911report/chapter-10.txt
./911report/chapter-11.txt
./911report/chapter-12.txt
./911report/chapter-13.1.txt
./911report/chapter-13.2.txt
./biomed/1471-2091-2-10.txt
./biomed/1471-2091-2-11.txt
./biomed/1471-2091-2-12.txt
./biomed/1471-2091-2-13.txt
./biomed/1471-2091-2-16.txt
```
Type -f searches for all *file* types within the directory, very useful for searching
for specific types of data.



*find -type d*
```
$ find -type d
.
./911report
./biomed
./government
./government/About_LSC
./government/Alcohol_Problems
./government/Env_Prot_Agen
./government/Gen_Account_Office
./government/Media
./government/Post_Rate_Comm
./plos
```
Type -d searches for *directory* types within the directory which is useful to differentiate
directories and files.


**2. -name**

```
$ find -name "*.0020281.txt"
./plos/pmed.0020281.txt
```
Find -name allows one to search for specific contents of a file, allowing one to quickly
find specific files or directories.

```
$ find -name "plos"
./plos
```
Searches for a file containing the string "plos", which quickly allows me to determine
whether the directory contains a certain file/directory.


**3. -path**
```
$ find -path "*.txt"
./911report/chapter-1.txt
./911report/chapter-10.txt
./911report/chapter-11.txt
./911report/chapter-12.txt
./911report/chapter-13.1.txt
./911report/chapter-13.2.txt
./911report/chapter-13.3.txt
./911report/chapter-13.4.txt
./911report/chapter-13.5.txt
./911report/chapter-2.txt
./911report/chapter-3.txt
./911report/chapter-5.txt
```
Extremely similar to -name, however it allows you to also include the entire path instead of just
the file name.


```
$ find -path "*0.txt"
./journal.pbio.0020010.txt
./journal.pbio.0020040.txt
./journal.pbio.0020100.txt
./journal.pbio.0020140.txt
./journal.pbio.0020150.txt
./journal.pbio.0020190.txt
./journal.pbio.0020310.txt
./journal.pbio.0020350.txt
./journal.pbio.0020400.txt
./journal.pbio.0020420.txt
./journal.pbio.0020430.txt
./journal.pbio.0020440.txt
./journal.pbio.0030050.txt
./pmed.0010010.txt
./pmed.0010030.txt
./pmed.0010050.txt
./pmed.0010060.txt
./pmed.0010070.txt
./pmed.0020020.txt
./pmed.0020040.txt
```
Allows you to search for more than just the file name and able to trace back through
multiple directories.



4. **-and**
```
$ find -name "*.txt" -type f
./chapter-1.txt
./chapter-10.txt
./chapter-11.txt
./chapter-12.txt
./chapter-13.1.txt
./chapter-13.2.txt
./chapter-13.3.txt
./chapter-13.4.txt
./chapter-13.5.txt
./chapter-2.txt
./chapter-3.txt
./chapter-5.txt
./chapter-6.txt
./chapter-7.txt
./chapter-8.txt
./chapter-9.txt
./preface.txt
```
Allows one to combine multiple commands such as both -name and -type within the same search,
which is helpful to further hone down the scope of a search.


```
$ find -name "*s" -type d
./Alcohol_Problems
```
Quickly was able to determine if a directory with the last letter of s existed within a certain folder.


### Source/Reference
[Github BashFind Command](https://math2001.github.io/article/bashs-find-command/)

[Base-Name-Patterns](https://www.gnu.org/software/findutils/manual/html_mono/find.html#Base-Name-Patterns)
