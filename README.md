# cargo-geiger Format Issue

Run with

```sh
cargo geiger --all-dependencies --include-tests
```

to get

```sh
Functions  Expressions  Impls  Traits  Methods  Dependency

0/0        0/0          0/0    0/0     0/0      ❓ cargo-geiger-issue 0.1.0
0/0        0/0          0/0    0/0     0/0      ❓ └── color-eyre 0.5.11
11/22      334/785      2/6    0/0     0/5      ☢️     ├── backtrace 0.3.63
                                                           │   [build-dependencies]
1/1        194/194      2/2    0/0     4/4      ☢️     │   └── cc 1.0.72
0/0        11/26        0/0    0/0     0/0      ☢️     │   ├── addr2line 0.17.0
                                                           │   │   [dev-dependencies]
11/22      334/785      2/6    0/0     0/5      ☢️     │   │   └── backtrace 0.3.63
0/0        29/50        1/3    1/1     0/0      ☢️     │   │   ├── gimli 0.26.1
                                                           │   │   │   [dev-dependencies]
0/0        24/26        0/0    1/1     0/0      ☢️     │   │   │   └── object 0.27.1
20/37      1350/2171    0/0    0/0     16/16    ☢️     │   │   │       └── memchr 2.4.1
0/20       0/327        0/2    0/0     0/30     ❓     │   │   │           └── libc 0.2.112
0/0        24/26        0/0    1/1     0/0      ☢️     │   │   ├── object 0.27.1
0/0        0/0          0/0    0/0     0/0      ❓     │   │   └── rustc-demangle 0.1.21
0/0        0/0          0/0    0/0     0/0      ❓     │   ├── cfg-if 1.0.0
0/20       0/327        0/2    0/0     0/30     ❓     │   ├── libc 0.2.112
0/0        0/0          0/0    0/0     0/0      🔒     │   ├── miniz_oxide 0.4.4
                                                           │   │   [build-dependencies]
0/0        0/0          0/0    0/0     0/0      ❓     │   │   └── autocfg 1.0.1
0/0        0/0          0/0    0/0     0/0      🔒     │   │   └── adler 1.0.2
0/0        24/26        0/0    1/1     0/0      ☢️     │   ├── object 0.27.1
0/0        0/0          0/0    0/0     0/0      ❓     │   └── rustc-demangle 0.1.21
0/0        0/0          0/0    0/0     0/0      ❓     ├── color-spantrace 0.1.6
                                                           │   [dev-dependencies]
0/0        0/0          1/1    0/0     0/0      ☢️     │   ├── tracing 0.1.29
0/0        0/0          0/0    0/0     0/0      ❓     │   │   ├── cfg-if 1.0.0
0/0        11/165       0/0    0/0     2/2      ☢️     │   │   ├── pin-project-lite 0.2.8
0/0        0/0          0/0    0/0     0/0      ❓     │   │   ├── tracing-attributes 0.1.18
0/0        12/12        0/0    0/0     3/3      ☢️     │   │   │   ├── proc-macro2 1.0.36
0/0        0/0          0/0    0/0     0/0      🔒     │   │   │   │   └── unicode-xid 0.2.2
                                                           │   │   │   │   [dev-dependencies]
0/0        0/0          0/0    0/0     0/0      ❓     │   │   │   │   └── quote 1.0.14
0/0        12/12        0/0    0/0     3/3      ☢️     │   │   │   │       └── proc-macro2 1.0.36
0/0        0/0          0/0    0/0     0/0      ❓     │   │   │   ├── quote 1.0.14
0/0        47/47        3/3    0/0     2/2      ☢️     │   │   │   └── syn 1.0.85
0/0        12/12        0/0    0/0     3/3      ☢️     │   │   │       ├── proc-macro2 1.0.36
0/0        0/0          0/0    0/0     0/0      ❓     │   │   │       ├── quote 1.0.14
0/0        0/0          0/0    0/0     0/0      🔒     │   │   │       └── unicode-xid 0.2.2
                                                           │   │   │   [dev-dependencies]
0/0        0/0          1/1    0/0     0/0      ☢️     │   │   │   ├── tracing 0.1.29
0/0        36/57        0/4    0/0     2/2      ☢️     │   │   │   └── tracing-core 0.1.21
0/0        7/7          1/1    0/0     0/0      ☢️     │   │   │       └── lazy_static 1.4.0
0/0        36/57        0/4    0/0     2/2      ☢️     │   │   └── tracing-core 0.1.21
0/0        115/129      1/1    0/0     6/7      ☢️     │   └── tracing-subscriber 0.2.25
                                                           │       [dev-dependencies]
0/0        0/0          1/1    0/0     0/0      ☢️     │       └── tracing 0.1.29
0/0        162/162      10/10  0/0     8/8      ☢️     │       ├── sharded-slab 0.1.4
0/0        7/7          1/1    0/0     0/0      ☢️     │       │   └── lazy_static 1.4.0
0/0        109/109      1/1    0/0     4/4      ☢️     │       ├── thread_local 1.1.3
1/1        86/106       4/6    0/0     2/3      ☢️     │       │   └── once_cell 1.9.0
                                                           │       │       [dev-dependencies]
0/0        7/7          1/1    0/0     0/0      ☢️     │       │       └── lazy_static 1.4.0
0/0        0/0          1/1    0/0     0/0      ☢️     │       ├── tracing 0.1.29
1/1        86/106       4/6    0/0     2/3      ☢️     │   ├── once_cell 1.9.0
0/0        0/8          0/0    0/0     0/0      ❓     │   ├── owo-colors 1.3.0
0/0        36/57        0/4    0/0     2/2      ☢️     │   ├── tracing-core 0.1.21
1/1        34/34        0/0    0/0     1/1      ☢️     │   └── tracing-error 0.1.2
0/0        0/0          1/1    0/0     0/0      ☢️     │       ├── tracing 0.1.29
0/0        115/129      1/1    0/0     6/7      ☢️     │       └── tracing-subscriber 0.2.25
10/10      222/222      0/0    0/0     1/1      ☢️     ├── eyre 0.6.5
0/0        0/0          0/0    0/0     0/0      ❓     │   ├── indenter 0.3.3
1/1        86/106       4/6    0/0     2/3      ☢️     │   └── once_cell 1.9.0
                                                           │   [dev-dependencies]
11/22      334/785      2/6    0/0     0/5      ☢️     │   └── backtrace 0.3.63
0/0        0/0          0/0    0/0     0/0      ❓     ├── indenter 0.3.3
1/1        86/106       4/6    0/0     2/3      ☢️     ├── once_cell 1.9.0
0/0        0/8          0/0    0/0     0/0      ❓     ├── owo-colors 1.3.0
1/1        34/34        0/0    0/0     1/1      ☢️     └── tracing-error 0.1.2
                                                           [dev-dependencies]
0/0        0/0          1/1    0/0     0/0      ☢️     ├── tracing 0.1.29
0/0        115/129      1/1    0/0     6/7      ☢️     └── tracing-subscriber 0.2.25

44/92      2783/4637    26/40  2/2     51/88

error: Found 67 warnings
```
