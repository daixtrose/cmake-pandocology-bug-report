# cmake-pandocology-bug-report
A small demo of the issue I currently have with pandocology

```
Microsoft Windows [Version 10.0.10586]
(c) 2015 Microsoft Corporation. Alle Rechte vorbehalten.

C:\Users\Markus>cd Documents\GitHub\cmake-pandocology-bug-report

C:\Users\Markus\Documents\GitHub\cmake-pandocology-bug-report>cd LaTeX\build

C:\Users\Markus\Documents\GitHub\cmake-pandocology-bug-report\LaTeX\build>cmake -G "MinGW Makefiles" ..
-- Configuring done
-- Generating done
-- Build files have been written to: C:/Users/Markus/Documents/GitHub/cmake-pandocology-bug-report/LaTeX/build

C:\Users\Markus\Documents\GitHub\cmake-pandocology-bug-report\LaTeX\build>make
Der Befehl "make" ist entweder falsch geschrieben oder
konnte nicht gefunden werden.

C:\Users\Markus\Documents\GitHub\cmake-pandocology-bug-report\LaTeX\build>"C:\Program Files (x86)\GnuWin32\bin\make.exe"
Scanning dependencies of target test.tex
[ 33%] Generating test.md
make[2]: Zirkuläre Datei CMakeFiles/test.tex <- test.tex Abhängigkeit wird nicht verwendet.
[ 66%] Generating product/test.tex
Error copying file "test.tex" to "C:/Users/Markus/Documents/GitHub/cmake-pandocology-bug-report/LaTeX/build/product".
make[2]: *** [product/test.tex] Fehler 1
make[1]: *** [CMakeFiles/test.tex.dir/all] Fehler 2
make: *** [all] Fehler 2
```
