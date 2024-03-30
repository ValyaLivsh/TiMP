# TiMP
# RK1 - Llama2
# Have you ever wanted to inference a baby Llama 2 model in pure C? No? Well, now you can!
# 3. Количество файлов 
```
ls . | wc -l
23
```
# 4. Объём всех файлов
```
du -h -a /home/valya/llama2.c
4,0K	/home/valya/llama2.c/doc/stories260K.md
4,0K	/home/valya/llama2.c/doc/train_llama_tokenizer.md
12K	/home/valya/llama2.c/doc
4,0K	/home/valya/llama2.c/run.ipynb
12K	/home/valya/llama2.c/tinystories.py
4,0K	/home/valya/llama2.c/test.c
184K	/home/valya/llama2.c/assets/llama_cute.jpg
188K	/home/valya/llama2.c/assets
492K	/home/valya/llama2.c/tokenizer.model
4,0K	/home/valya/llama2.c/Makefile
424K	/home/valya/llama2.c/tokenizer.bin
4,0K	/home/valya/llama2.c/win.h
4,0K	/home/valya/llama2.c/test_all.py
4,0K	/home/valya/llama2.c/.git/refs/tags
4,0K	/home/valya/llama2.c/.git/refs/heads/master
8,0K	/home/valya/llama2.c/.git/refs/heads
4,0K	/home/valya/llama2.c/.git/refs/remotes/origin/HEAD
8,0K	/home/valya/llama2.c/.git/refs/remotes/origin
12K	/home/valya/llama2.c/.git/refs/remotes
28K	/home/valya/llama2.c/.git/refs
4,0K	/home/valya/llama2.c/.git/info/exclude
8,0K	/home/valya/llama2.c/.git/info
4,0K	/home/valya/llama2.c/.git/logs/refs/heads/master
8,0K	/home/valya/llama2.c/.git/logs/refs/heads
4,0K	/home/valya/llama2.c/.git/logs/refs/remotes/origin/HEAD
8,0K	/home/valya/llama2.c/.git/logs/refs/remotes/origin
12K	/home/valya/llama2.c/.git/logs/refs/remotes
24K	/home/valya/llama2.c/.git/logs/refs
4,0K	/home/valya/llama2.c/.git/logs/HEAD
32K	/home/valya/llama2.c/.git/logs
4,0K	/home/valya/llama2.c/.git/objects/info
1,3M	/home/valya/llama2.c/.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.pack
44K	/home/valya/llama2.c/.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.idx
1,3M	/home/valya/llama2.c/.git/objects/pack
1,3M	/home/valya/llama2.c/.git/objects
4,0K	/home/valya/llama2.c/.git/packed-refs
4,0K	/home/valya/llama2.c/.git/branches
4,0K	/home/valya/llama2.c/.git/config
8,0K	/home/valya/llama2.c/.git/hooks/pre-rebase.sample
4,0K	/home/valya/llama2.c/.git/hooks/commit-msg.sample
4,0K	/home/valya/llama2.c/.git/hooks/pre-applypatch.sample
4,0K	/home/valya/llama2.c/.git/hooks/post-update.sample
4,0K	/home/valya/llama2.c/.git/hooks/pre-commit.sample
4,0K	/home/valya/llama2.c/.git/hooks/applypatch-msg.sample
4,0K	/home/valya/llama2.c/.git/hooks/push-to-checkout.sample
4,0K	/home/valya/llama2.c/.git/hooks/update.sample
4,0K	/home/valya/llama2.c/.git/hooks/pre-push.sample
4,0K	/home/valya/llama2.c/.git/hooks/pre-merge-commit.sample
8,0K	/home/valya/llama2.c/.git/hooks/fsmonitor-watchman.sample
4,0K	/home/valya/llama2.c/.git/hooks/prepare-commit-msg.sample
4,0K	/home/valya/llama2.c/.git/hooks/pre-receive.sample
64K	/home/valya/llama2.c/.git/hooks
4,0K	/home/valya/llama2.c/.git/description
4,0K	/home/valya/llama2.c/.git/index
4,0K	/home/valya/llama2.c/.git/HEAD
1,5M	/home/valya/llama2.c/.git
40K	/home/valya/llama2.c/run.c
4,0K	/home/valya/llama2.c/sample.py
36K	/home/valya/llama2.c/README.md
16K	/home/valya/llama2.c/train.py
4,0K	/home/valya/llama2.c/LICENSE
24K	/home/valya/llama2.c/export.py
4,0K	/home/valya/llama2.c/build_msvc.bat
8,0K	/home/valya/llama2.c/win.c
4,0K	/home/valya/llama2.c/configurator.py
4,0K	/home/valya/llama2.c/tokenizer.py
44K	/home/valya/llama2.c/runq.c
4,0K	/home/valya/llama2.c/requirements.txt
16K	/home/valya/llama2.c/model.py
8,0K	/home/valya/llama2.c/.github/workflows/build.yml
12K	/home/valya/llama2.c/.github/workflows
16K	/home/valya/llama2.c/.github
2,8M	/home/valya/llama2.c
```
# 5. Объём исходного кода
```
wc -l $(find . -type f -name '*.py' -o -name '*.c' -o -name '*.h') | tail -1  
  4225 total
```
# 6. Найти, если есть файл .clang-format
```
find . -type f -name '*.clang-format'

```
# 7. Если есть файл src, общее количество файлов в каталоге src
```
cd /usr/src
/usr/src$ ls . | wc -l
4
```
# 8. Выписать количество файлов, содержащих слово socket 
```
grep -irm 1 socket . | wc -l
grep: ./tokenizer.model: binary file matches
grep: ./tokenizer.bin: binary file matches
0
```
# 9. Выписать количество файлов содержащих слово select
```
grep -irm 1 select . | wc -l
grep: ./tokenizer.model: binary file matches
grep: ./tokenizer.bin: binary file matches
2
```
# 10. Выписать количество раз, сколько содержится слово Microsoft, Google или Intel во всех файлах репозитория 
```
grep -c -R 'microsoft'
doc/stories260K.md:0
doc/train_llama_tokenizer.md:0
run.ipynb:0
tinystories.py:0
test.c:0
assets/llama_cute.jpg:0
tokenizer.model:1
Makefile:0
tokenizer.bin:1
win.h:0
test_all.py:0
.git/refs/heads/master:0
.git/refs/remotes/origin/HEAD:0
.git/info/exclude:0
.git/logs/refs/heads/master:0
.git/logs/refs/remotes/origin/HEAD:0
.git/logs/HEAD:0
.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.pack:0
.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.idx:0
.git/packed-refs:0
.git/config:0
.git/hooks/pre-rebase.sample:0
.git/hooks/commit-msg.sample:0
.git/hooks/pre-applypatch.sample:0
.git/hooks/post-update.sample:0
.git/hooks/pre-commit.sample:0
.git/hooks/applypatch-msg.sample:0
.git/hooks/push-to-checkout.sample:0
.git/hooks/update.sample:0
.git/hooks/pre-push.sample:0
.git/hooks/pre-merge-commit.sample:0
.git/hooks/fsmonitor-watchman.sample:0
.git/hooks/prepare-commit-msg.sample:0
.git/hooks/pre-receive.sample:0
.git/description:0
.git/index:0
.git/HEAD:0
run.c:0
sample.py:0
README.md:0
train.py:0
LICENSE:0
export.py:0
build_msvc.bat:0
win.c:0
configurator.py:0
tokenizer.py:0
runq.c:0
requirements.txt:0
model.py:0
.github/workflows/build.yml:1

grep -c -R 'google'
doc/stories260K.md:0
doc/train_llama_tokenizer.md:1
run.ipynb:1
tinystories.py:0
test.c:0
assets/llama_cute.jpg:0
tokenizer.model:3
Makefile:0
tokenizer.bin:3
win.h:0
test_all.py:0
.git/refs/heads/master:0
.git/refs/remotes/origin/HEAD:0
.git/info/exclude:0
.git/logs/refs/heads/master:0
.git/logs/refs/remotes/origin/HEAD:0
.git/logs/HEAD:0
.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.pack:0
.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.idx:0
.git/packed-refs:0
.git/config:0
.git/hooks/pre-rebase.sample:0
.git/hooks/commit-msg.sample:0
.git/hooks/pre-applypatch.sample:0
.git/hooks/post-update.sample:0
.git/hooks/pre-commit.sample:0
.git/hooks/applypatch-msg.sample:0
.git/hooks/push-to-checkout.sample:0
.git/hooks/update.sample:0
.git/hooks/pre-push.sample:0
.git/hooks/pre-merge-commit.sample:0
.git/hooks/fsmonitor-watchman.sample:0
.git/hooks/prepare-commit-msg.sample:0
.git/hooks/pre-receive.sample:0
.git/description:0
.git/index:0
.git/HEAD:0
run.c:0
sample.py:0
README.md:1
train.py:0
LICENSE:0
export.py:0
build_msvc.bat:0
win.c:0
configurator.py:0
tokenizer.py:0
runq.c:0
requirements.txt:0
model.py:0
.github/workflows/build.yml:0

grep -c -R 'intel'
doc/stories260K.md:0
doc/train_llama_tokenizer.md:0
run.ipynb:0
tinystories.py:0
test.c:0
assets/llama_cute.jpg:0
tokenizer.model:6
Makefile:0
tokenizer.bin:6
win.h:0
test_all.py:0
.git/refs/heads/master:0
.git/refs/remotes/origin/HEAD:0
.git/info/exclude:0
.git/logs/refs/heads/master:0
.git/logs/refs/remotes/origin/HEAD:0
.git/logs/HEAD:0
.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.pack:0
.git/objects/pack/pack-6d0bd05dad82d25faa130ce00cbfef550ea5add4.idx:0
.git/packed-refs:0
.git/config:0
.git/hooks/pre-rebase.sample:0
.git/hooks/commit-msg.sample:0
.git/hooks/pre-applypatch.sample:0
.git/hooks/post-update.sample:0
.git/hooks/pre-commit.sample:0
.git/hooks/applypatch-msg.sample:0
.git/hooks/push-to-checkout.sample:0
.git/hooks/update.sample:0
.git/hooks/pre-push.sample:0
.git/hooks/pre-merge-commit.sample:0
.git/hooks/fsmonitor-watchman.sample:0
.git/hooks/prepare-commit-msg.sample:0
.git/hooks/pre-receive.sample:0
.git/description:0
.git/index:0
.git/HEAD:0
run.c:0
sample.py:0
README.md:0
train.py:0
LICENSE:0
export.py:0
build_msvc.bat:0
win.c:0
configurator.py:0
tokenizer.py:0
runq.c:0
requirements.txt:0
model.py:0
.github/workflows/build.yml:0
```
# 11. Найти расположение файла LICENSE относительно начала репозитория
```
git ls-files --full-name LICENSE
LICENSE
```
# 12. Вывести строку для файла LICENSE (если он есть), содержащую следующие подпоследовательности символов: BSD, GNU, MIT, APSL, Apache, GPL, AGPL, LGPL
```
grep -rn --include="LICENSE" "BSD\|GNU\|MIT\|APSL\|Apache\|GPL\|AGPL\|LGPL" .
./LICENSE:1:MIT License
./LICENSE:16:IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
```
