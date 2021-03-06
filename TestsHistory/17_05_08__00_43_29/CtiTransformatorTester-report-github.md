``` ini

BenchmarkDotNet=v0.10.5, OS=Windows 10.0.15063
Processor=Intel Core i7-4710MQ CPU 2.50GHz (Haswell), ProcessorCount=8
Frequency=2435773 Hz, Resolution=410.5473 ns, Timer=TSC
  [Host]            : Clr 4.0.30319.42000, 32bit LegacyJIT-v4.7.2046.0
  LegacyJit-Clr-X64 : Clr 4.0.30319.42000, 64bit LegacyJIT/clrjit-v4.7.2046.0;compatjit-v4.7.2046.0
  LegacyJit-Clr-X86 : Clr 4.0.30319.42000, 32bit LegacyJIT-v4.7.2046.0
  RyuJit-Clr-X64    : Clr 4.0.30319.42000, 64bit RyuJIT-v4.7.2046.0
  RyuJit-Clr-X86    : Clr 4.0.30319.42000, 32bit LegacyJIT-v4.7.2046.0

Runtime=Clr  

```
 |                    Method |               Job |       Jit | Platform |      Mean |     Error |    StdDev | Scaled |     Gen 0 | Allocated |
 |-------------------------- |------------------ |---------- |--------- |----------:|----------:|----------:|-------:|----------:|----------:|
 |  Test_v_0_1_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 | 39.693 ms | 0.1682 ms | 0.1491 ms |   1.00 | 7308.3333 |   23.8 MB |
 |  Test_v_0_2_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 | 12.837 ms | 0.0422 ms | 0.0353 ms |   0.32 | 2964.5833 |    9.3 MB |
 |  Test_v_0_3_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 | 11.538 ms | 0.0453 ms | 0.0423 ms |   0.29 | 2163.5417 |   6.94 MB |
 |  Test_v_0_4_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 | 11.583 ms | 0.0528 ms | 0.0494 ms |   0.29 | 2138.5417 |   6.94 MB |
 |  Test_v_0_5_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  6.424 ms | 0.0188 ms | 0.0166 ms |   0.16 | 1794.7917 |    5.6 MB |
 |  Test_v_0_6_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  5.419 ms | 0.0143 ms | 0.0127 ms |   0.14 | 2280.7292 |   7.06 MB |
 |  Test_v_0_7_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  3.769 ms | 0.0212 ms | 0.0199 ms |   0.09 | 2222.1354 |   6.79 MB |
 |  Test_v_0_8_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  3.588 ms | 0.0075 ms | 0.0071 ms |   0.09 | 1608.8542 |   4.95 MB |
 |  Test_v_0_9_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.707 ms | 0.0083 ms | 0.0078 ms |   0.07 | 1609.8958 |   4.95 MB |
 | Test_v_0_10_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.514 ms | 0.0122 ms | 0.0114 ms |   0.06 | 1609.8958 |   4.95 MB |
 | Test_v_0_11_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.482 ms | 0.0086 ms | 0.0080 ms |   0.06 | 1608.8542 |   4.95 MB |
 | Test_v_0_12_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.666 ms | 0.0102 ms | 0.0095 ms |   0.07 | 1854.1667 |   5.68 MB |
 |  Test_v_1_1_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.855 ms | 0.0125 ms | 0.0110 ms |   0.07 | 1609.8958 |   4.95 MB |
 |  Test_v_1_2_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.689 ms | 0.0115 ms | 0.0107 ms |   0.07 | 1609.8958 |   4.95 MB |
 |  Test_v_2_0_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  2.484 ms | 0.0085 ms | 0.0079 ms |   0.06 | 1602.6042 |   4.95 MB |
 |  Test_v_3_0_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  3.487 ms | 0.0130 ms | 0.0121 ms |   0.09 | 1313.0208 |   4.06 MB |
 |  Test_v_4_0_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  5.274 ms | 0.0276 ms | 0.0258 ms |   0.13 | 1263.5417 |      4 MB |
 |  Test_v_4_1_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  5.219 ms | 0.0191 ms | 0.0178 ms |   0.13 | 1263.5417 |      4 MB |
 |  Test_v_4_2_transformator | LegacyJit-Clr-X64 | LegacyJit |      X64 |  4.388 ms | 0.0317 ms | 0.0264 ms |   0.11 |  933.3333 |   3.02 MB |
 |  Test_v_0_1_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 | 38.067 ms | 0.1731 ms | 0.1446 ms |   1.00 | 4758.3333 |  16.31 MB |
 |  Test_v_0_2_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 | 11.260 ms | 0.0358 ms | 0.0335 ms |   0.30 | 2417.7083 |   7.69 MB |
 |  Test_v_0_3_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  9.745 ms | 0.0354 ms | 0.0331 ms |   0.26 | 1831.2500 |   5.91 MB |
 |  Test_v_0_4_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  9.768 ms | 0.0493 ms | 0.0462 ms |   0.26 | 1831.2500 |   5.91 MB |
 |  Test_v_0_5_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  5.550 ms | 0.0195 ms | 0.0182 ms |   0.15 | 1545.8333 |   4.88 MB |
 |  Test_v_0_6_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  5.157 ms | 0.0224 ms | 0.0209 ms |   0.14 | 2029.1667 |   6.29 MB |
 |  Test_v_0_7_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  3.804 ms | 0.0105 ms | 0.0093 ms |   0.10 | 1996.8750 |    6.1 MB |
 |  Test_v_0_8_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  3.343 ms | 0.0662 ms | 0.0736 ms |   0.09 | 1400.7813 |   4.33 MB |
 |  Test_v_0_9_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.455 ms | 0.0098 ms | 0.0092 ms |   0.06 | 1404.9479 |   4.33 MB |
 | Test_v_0_10_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.435 ms | 0.0246 ms | 0.0206 ms |   0.06 | 1401.8229 |   4.33 MB |
 | Test_v_0_11_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.429 ms | 0.0081 ms | 0.0076 ms |   0.06 | 1402.8646 |   4.33 MB |
 | Test_v_0_12_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.561 ms | 0.0127 ms | 0.0119 ms |   0.07 | 1522.9167 |   4.69 MB |
 |  Test_v_1_1_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.390 ms | 0.0073 ms | 0.0069 ms |   0.06 | 1405.9896 |   4.33 MB |
 |  Test_v_1_2_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.424 ms | 0.0059 ms | 0.0046 ms |   0.06 | 1401.8229 |   4.33 MB |
 |  Test_v_2_0_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  2.947 ms | 0.0108 ms | 0.0095 ms |   0.08 | 1404.9479 |   4.33 MB |
 |  Test_v_3_0_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  3.428 ms | 0.0121 ms | 0.0113 ms |   0.09 | 1107.8125 |   3.46 MB |
 |  Test_v_4_0_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  5.048 ms | 0.0995 ms | 0.0931 ms |   0.13 |  930.7292 |   3.04 MB |
 |  Test_v_4_1_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  5.210 ms | 0.0383 ms | 0.0340 ms |   0.14 |  930.7292 |   3.04 MB |
 |  Test_v_4_2_transformator | LegacyJit-Clr-X86 | LegacyJit |      X86 |  3.932 ms | 0.0221 ms | 0.0207 ms |   0.10 |  712.5000 |   2.35 MB |
 |  Test_v_0_1_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 | 39.947 ms | 0.1297 ms | 0.1214 ms |   1.00 | 7325.0000 |   23.8 MB |
 |  Test_v_0_2_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 | 12.876 ms | 0.0700 ms | 0.0654 ms |   0.32 | 2964.5833 |    9.3 MB |
 |  Test_v_0_3_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 | 11.731 ms | 0.1396 ms | 0.1237 ms |   0.29 | 2167.7083 |   6.94 MB |
 |  Test_v_0_4_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 | 11.694 ms | 0.0364 ms | 0.0341 ms |   0.29 | 2151.0417 |   6.94 MB |
 |  Test_v_0_5_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  6.513 ms | 0.1231 ms | 0.1317 ms |   0.16 | 1784.3750 |    5.6 MB |
 |  Test_v_0_6_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  5.542 ms | 0.0258 ms | 0.0241 ms |   0.14 | 2280.7292 |   7.06 MB |
 |  Test_v_0_7_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  3.902 ms | 0.0099 ms | 0.0088 ms |   0.10 | 2223.1771 |   6.79 MB |
 |  Test_v_0_8_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  3.475 ms | 0.0114 ms | 0.0107 ms |   0.09 | 1608.8542 |   4.95 MB |
 |  Test_v_0_9_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.545 ms | 0.0069 ms | 0.0064 ms |   0.06 | 1605.7292 |   4.95 MB |
 | Test_v_0_10_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.512 ms | 0.0079 ms | 0.0074 ms |   0.06 | 1609.8958 |   4.95 MB |
 | Test_v_0_11_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.498 ms | 0.0105 ms | 0.0099 ms |   0.06 | 1609.8958 |   4.95 MB |
 | Test_v_0_12_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.646 ms | 0.0078 ms | 0.0073 ms |   0.07 | 1854.1667 |   5.68 MB |
 |  Test_v_1_1_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.585 ms | 0.0074 ms | 0.0062 ms |   0.06 | 1608.8542 |   4.95 MB |
 |  Test_v_1_2_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.622 ms | 0.0106 ms | 0.0100 ms |   0.07 | 1607.8125 |   4.95 MB |
 |  Test_v_2_0_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  2.492 ms | 0.0096 ms | 0.0075 ms |   0.06 | 1608.8542 |   4.95 MB |
 |  Test_v_3_0_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  3.536 ms | 0.0078 ms | 0.0073 ms |   0.09 | 1317.1875 |   4.06 MB |
 |  Test_v_4_0_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  4.905 ms | 0.0235 ms | 0.0220 ms |   0.12 | 1263.5417 |      4 MB |
 |  Test_v_4_1_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  4.843 ms | 0.0147 ms | 0.0138 ms |   0.12 | 1261.4583 |      4 MB |
 |  Test_v_4_2_transformator |    RyuJit-Clr-X64 |    RyuJit |      X64 |  4.031 ms | 0.0107 ms | 0.0083 ms |   0.10 |  929.1667 |   3.02 MB |
 |  Test_v_0_1_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 | 37.527 ms | 0.1466 ms | 0.1371 ms |   1.00 | 4808.3333 |  16.31 MB |
 |  Test_v_0_2_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 | 11.261 ms | 0.0349 ms | 0.0326 ms |   0.30 | 2396.8750 |   7.69 MB |
 |  Test_v_0_3_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  9.757 ms | 0.0585 ms | 0.0519 ms |   0.26 | 1835.4167 |   5.91 MB |
 |  Test_v_0_4_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  9.739 ms | 0.0440 ms | 0.0411 ms |   0.26 | 1835.4167 |   5.91 MB |
 |  Test_v_0_5_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  5.510 ms | 0.0202 ms | 0.0188 ms |   0.15 | 1552.0833 |   4.88 MB |
 |  Test_v_0_6_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  5.153 ms | 0.0306 ms | 0.0287 ms |   0.14 | 2012.5000 |   6.29 MB |
 |  Test_v_0_7_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  3.773 ms | 0.0099 ms | 0.0087 ms |   0.10 | 1990.6250 |    6.1 MB |
 |  Test_v_0_8_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  3.275 ms | 0.0083 ms | 0.0078 ms |   0.09 | 1398.6979 |   4.33 MB |
 |  Test_v_0_9_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.455 ms | 0.0085 ms | 0.0079 ms |   0.07 | 1404.9479 |   4.33 MB |
 | Test_v_0_10_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.422 ms | 0.0073 ms | 0.0068 ms |   0.06 | 1408.0729 |   4.33 MB |
 | Test_v_0_11_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.428 ms | 0.0087 ms | 0.0082 ms |   0.06 | 1403.9063 |   4.33 MB |
 | Test_v_0_12_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.557 ms | 0.0063 ms | 0.0056 ms |   0.07 | 1522.9167 |   4.69 MB |
 |  Test_v_1_1_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.406 ms | 0.0078 ms | 0.0069 ms |   0.06 | 1400.7813 |   4.33 MB |
 |  Test_v_1_2_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.411 ms | 0.0123 ms | 0.0096 ms |   0.06 | 1400.7813 |   4.33 MB |
 |  Test_v_2_0_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  2.950 ms | 0.0106 ms | 0.0099 ms |   0.08 | 1399.7396 |   4.33 MB |
 |  Test_v_3_0_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  3.404 ms | 0.0078 ms | 0.0073 ms |   0.09 | 1108.8542 |   3.46 MB |
 |  Test_v_4_0_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  4.975 ms | 0.0193 ms | 0.0181 ms |   0.13 |  920.3125 |   3.04 MB |
 |  Test_v_4_1_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  5.222 ms | 0.0175 ms | 0.0164 ms |   0.14 |  939.0625 |   3.04 MB |
 |  Test_v_4_2_transformator |    RyuJit-Clr-X86 |    RyuJit |      X86 |  3.923 ms | 0.0254 ms | 0.0238 ms |   0.10 |  746.8750 |   2.35 MB |
