# Vita3K iOS build report
- run: https://github.com/SSRplus/test/actions/runs/39903221818
- result: **failure**
- date: 2026-10-23 04:59 UTC

## Error lines
```
logs/01-get-source.log:14:ERROR: .gitmodules not found - is this the Vita3K source zip?
```

## 01-get-source.log (last 60 lines)
```
--- files in repo root:
total 31096
drwxr-xr-x  10 runner  staff      320 Oct 23 04:59 .
drwxr-xr-x   3 runner  staff       96 Oct 23 04:58 ..
drwxr-xr-x  14 runner  staff      448 Oct 23 04:59 .git
drwxr-xr-x   3 runner  staff       96 Oct 23 04:59 .github
drwxr-xr-x   3 runner  staff       96 Oct 23 04:59 logs
-rw-r--r--   1 runner  staff  7965539 Oct 23 04:59 project.zip
-rw-r--r--   1 runner  staff        6 Oct 23 04:59 README.md
-rw-r--r--   1 runner  staff    75769 Oct 23 04:59 Vita3K-iOS-port.zip
-rw-r--r--   1 runner  staff  7870306 Oct 23 04:59 Vita3K-Plus-master.zip
drwxr-xr-x   4 runner  staff      128 Oct 23 04:59 work
source zip: project.zip
ERROR: .gitmodules not found - is this the Vita3K source zip?
work/src_unz
work/src_unz/Vita3K-iOS-port
work/src_unz/Vita3K-iOS-port/build-ios.yml
work/src_unz/Vita3K-iOS-port/metal
work/src_unz/Vita3K-iOS-port/ios
work/src_unz/Vita3K-iOS-port/README.md
work/src_unz/Vita3K-iOS-port/scripts
work/src_unz/Vita3K-iOS-port/vita3k-ime
work/src_unz/Vita3K-Plus-master.zip
```
