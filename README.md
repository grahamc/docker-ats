# ats

```
root@docker:~/test# alias atscc="sudo docker run -v '$(pwd):/src' grahamc/ats $@"
root@docker:~/test# atscc ./test.dats
exec(patsopt --output test_dats.c --dynamic ./test.dats)
Hello from ATS2(ATS/Postiats)!
Loading [fixity.ats] starts!
Loading [fixity.ats] finishes!
Loading [basics_pre.sats] starts!
Loading [basics_pre.sats] finishes!
Loading [basics_sta.sats] starts!
Loading [basics_sta.sats] finishes!
Loading [basics_dyn.sats] starts!
Loading [basics_dyn.sats] finishes!
Loading [basics_gen.sats] starts!
Loading [basics_gen.sats] finishes!
The 1st translation (fixity) of [./test.dats] is successfully completed!
The 2nd translation (binding) of [./test.dats] is successfully completed!
The 3rd translation (type-checking) of [./test.dats] is successfully completed!
The 4th translation (type/proof-erasing) of [./test.dats] is successfully
completed!
exec(patsopt --output test_dats.c --dynamic ./test.dats) = 0
exec(gcc -std=c99 -D_XOPEN_SOURCE -I${PATSHOME} -I${PATSHOME}/ccomp/runtime
-L${PATSHOME}/ccomp/atslib/lib -L${PATSHOME}/ccomp/atslib/lib64  test_dats.c)
exec(gcc -std=c99 -D_XOPEN_SOURCE -I${PATSHOME} -I${PATSHOME}/ccomp/runtime
-L${PATSHOME}/ccomp/atslib/lib -L${PATSHOME}/ccomp/atslib/lib64  test_dats.c) =
0
```

