``` shell
$ ./db_bench
LevelDB:    version 1.23
Keys:       16 bytes each
Values:     100 bytes each (50 bytes after compression)
Entries:    1000000
RawSize:    110.6 MB (estimated)
FileSize:   62.9 MB (estimated)
WARNING: Snappy compression is not enabled
------------------------------------------------
fillseq      :       6.605 micros/op;   16.7 MB/s
fillsync     :   19086.418 micros/op;    0.0 MB/s (1000 ops)
fillrandom   :      13.616 micros/op;    8.1 MB/s
overwrite    :      19.044 micros/op;    5.8 MB/s
readrandom   :       4.839 micros/op; (864322 of 1000000 found)
readrandom   :       3.061 micros/op; (864083 of 1000000 found)
readseq      :       0.130 micros/op;  848.4 MB/s
readreverse  :       0.263 micros/op;  421.2 MB/s
compact      : 2013309.000 micros/op;
readrandom   :       2.266 micros/op; (864105 of 1000000 found)
readseq      :       0.110 micros/op; 1003.1 MB/s
readreverse  :       0.234 micros/op;  473.2 MB/s
fill100K     :    3213.376 micros/op;   29.7 MB/s (1000 ops)
crc32c       :       1.133 micros/op; 3448.2 MB/s (4K per op)
snappycomp   :    3853.000 micros/op; (snappy failure)
snappyuncomp :    2596.000 micros/op; (snappy failure)
```