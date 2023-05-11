# Lab Report 3

##The `find` Command
1. find -type

find -type f
```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical (main)
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

find -type d
```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical (main)
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

2. find -name
```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical (main)
$ find -name "*.0020281.txt"
./plos/pmed.0020281.txt
```

```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical (main)
$ find -name "plos"
./plos
```

3. find -path
```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical (main)
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

```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical/plos (main)
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
4. find -and
```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical/911report (main)
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

```
darka@kiichi MINGW64 ~/OneDrive/Documents/Github/docsearch/technical/government (main)
$ find -name "*s" -type d
./Alcohol_Problems
```
