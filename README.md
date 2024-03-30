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
readlink -f LICENSE
/home/valya/llama2.c/LICENSE
```
