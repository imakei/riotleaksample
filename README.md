# riotleaksample
Memory leak sample in Riotjs

## Setup
```
npm install .
```

## Build
```
npm run build
```

## Rund
```
npm run start
```

#Error
I got a following error.
```
<--- Last few GCs --->

   26707 ms: Scavenge 1397.9 (1456.9) -> 1397.9 (1456.9) MB, 0.8 / 0 ms (+ 2.0 ms in 1 steps since last GC) [allocation failure] [incremental marking delaying mark-sweep].
   27998 ms: Mark-sweep 1397.9 (1456.9) -> 1397.9 (1456.9) MB, 1291.4 / 0 ms (+ 3.1 ms in 2 steps since start of marking, biggest step 2.0 ms) [last resort gc].
   29299 ms: Mark-sweep 1397.9 (1456.9) -> 1397.8 (1456.9) MB, 1300.7 / 0 ms [last resort gc].


<--- JS stacktrace --->

==== JS stack trace =========================================

Security context: 0x28008fe37339 <JS Object>
    1: observable [/path/to/riotleaksample/node_modules/riot/riot.js:~30] [pc=0x35cf9ea707e2] (this=0x2c6d46b77769 <an Object with map 0x38cfa5d394d1>,el=0x28008feb7139 <a Tag with map 0x38cfa5d445d9>)
    2: new constructor(aka Tag) [/path/to/riotleaksample/node_modules/riot/riot.js:~646] [pc=0x35cf9ea70a6b] (this=0x28008feb71...

FATAL ERROR: CALL_AND_RETRY_LAST Allocation failed - process out of memory
```


