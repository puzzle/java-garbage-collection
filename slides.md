---
title: Java Garbage Collection
---

<!-- .slide: class="master01" -->

# Java<br/>Garbage<br/>Collection

---

<!-- .slide: class="master02" -->

# Overview

* -XX:+UseStringDeduplication
* einem Vergleich dieser inkl. Tradeoffs,
* die Wichtisten Optionen inkl. Defaults,
* Auswahlhilfe inkl. Tools,
* Java GCs in Containern,
* Allenfalls einige Details zu einem der neueren GCs
* ZGC 
* Escape analysis
* GC Generations
* Java Ergonomics 

---

<!-- .slide: class="text-left" -->
## What does a GC do?

* Tracks every object in JVM Heap
* Removes unused objects

---

<!-- .slide: class="text-left" -->
## GC Advantages

* No manual memory allocation
* No dangling pointers
* Fewer memory leaks

---

<!-- .slide: class="text-left" -->
## GC Disadvantages

* Additional CPU power required
* Additional latency and possibly pauses
* No control over CPU scheduling for freeing memory

---

<!-- .slide: class="text-left" -->
## Java 8 Available GCs

* Serial Garbage Collector (default, `-XX:+UseSerialGC`)
* Parallel Garbage Collector (default, `XX:+UseParallelGC`)
* CMS Garbage Collector (`-XX:+UseConcMarkSweepGC`)
* G1 Gargbage Collector (`-XX:+UseG1GC`)

---

<!-- .slide: class="text-left" -->
## Java 11 Available GCs

* Serial Garbage Collector (default, `-XX:+UseSerialGC`)
* Parallel Garbage Collector (`XX:+UseParallelGC`)
* CMS Garbage Collector (deprecated, `-XX:+UseConcMarkSweepGC`)
* G1 Gargbage Collector (default, `-XX:+UseG1GC`)
* Z Garbage Collector (experimental, `-XX:+UseZGC`)

---

<!-- .slide: class="text-left" -->
## Summary

---

<!-- .slide: class="text-left" -->
## What's Next
