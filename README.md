# TiMP
# RK1 - Llama2
# Have you ever wanted to inference a baby Llama 2 model in pure C? No? Well, now you can!
# 1 
```
ls . | wc -l
23
```
# 2
```
du -a -h --max-depth=1 | sort -hr
2,8M	.
1,5M	./.git
492K	./tokenizer.model
424K	./tokenizer.bin
188K	./assets
44K	./runq.c
40K	./run.c
36K	./README.md
24K	./export.py
16K	./train.py
16K	./model.py
16K	./.github
12K	./tinystories.py
12K	./doc
8,0K	./win.c
4,0K	./win.h
4,0K	./tokenizer.py
4,0K	./test.c
4,0K	./test_all.py
4,0K	./sample.py
4,0K	./run.ipynb
4,0K	./requirements.txt
4,0K	./Makefile
4,0K	./LICENSE
4,0K	./configurator.py
4,0K	./build_msvc.bat
```
# 3 
```
wc -l $(find . -type f -name '*.py' -o -name '*.c' -o -name '*.h') | tail -1  
  4225 total
```
# 4
```
find . -type f -name '*.clang-format'

```
# 5
```
cd /usr/src
/usr/src$ ls . | wc -l
4
```
