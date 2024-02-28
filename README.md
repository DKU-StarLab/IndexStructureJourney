# IndexStructureJourney

2024 [DKU System Software Lab](https://sslab.dankook.ac.kr/) Index  Study

## Goals
* Study Index and Learned Index Structures
* Write a open-source document.
* (Optional) Write a research paper on what you learned.

## Schedule
### Paper Presentation
|         | Date      | Content                                                                               | Presenter                               |
| :------ | :-------- | :------------------------------------------------------------------------------------ | :-------------------------------------- |
| Week 1  | 24-01-03  | ["Traditional Index"](./presentation_file/W1_HojinShin.pdf)                                                                  | Hojin Shin                              |
| Week 2  | 24-01-10  | "Traditional Index"                                                                   | Hojin Shin                              |
|         |           | ["A Learned Index Journey"](./presentation_file/W2_MingukChoi_A_Index_Journey.pdf)                                                         | Minguk Choi                             |
| Week 3  | 24-01-17  | ["No Hot Spot Non-blocking Skip List", ICDCS 13](./presentation_file/W3_NakyeongKim_SuhwanShin.pptx)                                       | Nakyeong Kim, Suhwan Shin               |
| Week 4  | 24-01-24  | ["Benchmarking learned indexes.", VLDB 20](./presentation_file/W4_YeojinOh_ZhuYongjie.pptx)                                                | Yeojin Oh, Zhu Yongjie       |
|         |           | ["S3: A Scalable In-memory Skip-List Index for Key-Value Store", VLDB 19](./presentation_file/W4_BoseungKim_yeongyuChoi.pdf)               | Boseung Kim, Yeongyu Choi               |
| Week 5  | 24-01-31  | ["Learned Index: A Comprehensive Experimental Evaluation." VLDB 23](./presentation_file/W5_NakyeongKim_SuhwanShin_YeongyuChoi.pptx)                           | Nakyeong Kim, Suhwan Shin, Yeongyu Choi |
| Week 6  | 24-02-07  | Lunar New Year Holiday          | |
| Week 7  | 24-02-14  | ["Cache craftiness for fast multicore key-value storage", EuroSys '12](./presentation_file/W7_YeojinOh_ZhuYongJie_BosengKim_Masstree.pdf)          | Boseung Kim, Yeojin Oh, Zhu Yongjie     |
| Week 8  | 24-02-21  | ["The adaptive radix tree: ARTful indexing for main-memory databases", ICDE 13](./presentation_file/W8_NakyeongKim_SuhwanShin.pdf)               | Nakyeong Kim, Suhwan Shin |
| Week 9  | 24-02-28  | ["Film: A fully learned index for larger-than-memory databases", VLDB 23] (./presentation_file/W9_YeojinOh_ZhuYongJie_BoseungKim.pdf)                                        | Boseung Kim, Yeojin Oh, Zhu Yongjie     |


### Evaluation Presentation
|        |          | Presenter                               | Contents |
| :----- | :------- | :-------------------------------------- | :------- |
| Week 4 | 24-01-24 | Nakyeong Kim, Suhwan Shin               | [No Hot Spot Non-Blocking Skip List - Range Query Experiment](./presentation_file/W4_NakyeongKim_SuhwanShin.pdf) |
| Week 5 | 24-01-31 | Boseung Kim, Yeojin Oh, Zhu Yongjie     | [Apply SIMD to RMI](presentation_file/W5_YeojinOh_ZhuYongJie_BosengKim.pdf) |
| Week 6 | 24-02-07 | Lunar New Year Holiday                  |          |
| Week 7 | 24-02-14 | Nakyeong Kim, Suhwan Shin | [LIPP Observations](./presentation_file/W7_NakyeongKim_SuhwanShin.pdf) |
|        |          | Boseung Kim, Yeojin Oh, Zhu Yongjie     | [Applying SIMD in Linear Regression](./presentation_file/W7_YeojinOh_ZhuYongJie_BoseungKim_SIMD.pdf) |
| Week 8 | 24-02-21 | Nakyeong Kim, Suhwan Shin |[LIPP Observations Enhancement](./presentation_file/W8_NakyeongKim_SuhwanShin_experiment.pdf)|
|        |          | Boseung Kim, Yeojin Oh, Zhu Yongjie     |[SIMD + RMI](./presentation_file/W8_YeojinOh_ZhuYongJie_BoseungKim.pdf)          |
| Week 9 | 24-02-28 | Nakyeong Kim, Suhwan Shin | [LIPP New Hypothesis](./presentation_file/W9_NakyeongKim_SuhwanShin_experiment.pdf) |
|        |          | Boseung Kim, Yeojin Oh, Zhu Yongjie     | [Revisiting HW Parallelism in Learned Indexes](./presentation_file/W9_YeojinOh_ZhuYongJie_BoseungKim_experiment.pdf)
|

## Paper & Lecture List
### Benchmarks
- Traditional Index : [Index-Microbench](https://github.com/ErosBryant/new-index-microbench)
  - Traditional Index : SkipList, B+TreeRTM, B+TreeOLC, BwTree, ARTOLC, MassTree
- Read-Only Learned Index : [LIST](https://github.com/DKU-StarLab/Benchmark4Sampling)
  - Learned Index : sRMI, sPGM-Index, sRS
  - Traditional Index : sCHT, sRT, sB+Tree(STX B+-Tree), sART, sIBTree
- Updatable Learned Index : [GRE](https://github.com/gre4index/GRE)
  - Learned Index : ALEX, ALEX+, LIPP, LIPP+, PGM-Index, XIndex, FINEdex
  - Traditional Index : STX B+Tree, B+TreeOLC, ART, ART-OLC, HOT, HOT-ROWEX, MassTree, Wormhole

### Traditional Index
- Tree-based
  - Douglas Comer, "Ubiquitous B-Tree", ACM Computing Surveys, 1979
  - R. Bayer, et al. "Organization and maintenance of large ordered indices", SIGFIDET '70
  - Justin J. Levandoski, et al. "The Bw-Tree: A B-tree for new hardware platform", ICDE 2013 [:octocat:](https://github.com/flode/BwTree.git)
  - J. Rao, et al. "Making B+-Trees Cache Conscious in Main Memory", SIGMOD 2000 [:octocat:](https://github.com/EmmanuelSHS/Cache_Sensitive_B_Tree.git)
  - J. Rao, et al. "Cache Conscious Indexing for Decision-Support in Main Memory", VLDB '99 [:octocat:](https://github.com/gvinciguerra/CSS-tree.git)
  - Changkyu Kim et al. "FAST: fast architecture sensitive tree search on modern CPUs and GPUs", SIGMOD '10
  - Yandong Mao, et al. "Cache craftiness for fast multicore key-value storage", EuroSys '12 [:octocat:](https://github.com/kohler/masstree-beta.git)
  - Viktor Leis, et al. "The adaptive radix tree: ARTful indexing for main-memory databases", ICDE 2013 [:octocat:](https://github.com/armon/libart.git)
  - Wook-Hee Kim, et al. "PACTree: A High Performance Persistent Range Index Using PAC Guidelines", SOSP '21 [:octocat:](https://github.com/cosmoss-jigu/pactree.git)
  - Se Kwon Lee, et al. "WORT: Write Optimal Radix Tree for Persistent Memory Storage Systems", FAST '17 [:octocat:](https://github.com/SeKwonLee/WORT.git)
- List-based
  - William Pugh, "Skip lists: a probabilistic alternative to balanced trees", Communications of the ACM 1990
  - Zhongle Xie, et al. "Parallelizing Skip Lits for In-Memory Multi-Core Database Systems", ICDE 2017
  - Jeseong Yeon, et al. "JellyFish: A Fast Skip List with MVCC", Middleware '20
  - Tyler Crain, et al. "No Hot Spot Non-blocking Skip List", ICDCS 2013
  - Henry Daly, et al. "NUMASK: High Performance Scalable Skip List for NUMA", DISC 2018 [:octocat:](https://github.com/sss-lehigh/numask.git)
  - Yedam Na, et al. "ESL: A High-Performance Skiplist with Express Lane", MDPI 2023
  - Zhongle Xie, et al. "PI: a parallel in-memory skip list based index", CoRR 2016
  - Tadeusz Kobus, et al. "Jiffy: a lock-free skip list with batch updates and snapshots", PPoPP '22 [:octocat:](https://github.com/tkobus/jiffy.git)
  - Vitaly Aksenov, et al. "The splay-list: a distribution-adaptive concurrent skip-list", Distributed Computing 2023
- Hash-based
  - Tudor David, et al. "Asynchronized Concurrency: The Secret to Scaling Concurrent Search Data Structures", ACM SGARCH '15 [:octocat:](https://github.com/LPD-EPFL/CLHT.git)
  - Vikram Narayanan, et al. "DRAMHiT: A Hash Table Architected for the Speed of DRAM", EuroSys '23
  - Daokun Hu, et al. "Halo: A Hybrid PMem-DRAM Persistent Hash Index with Fast Recovery", SIGMOD '20 [:octocat:](https://github.com/HNUSystemsLab/Halo.git)
- Hybrid Technique
  - Jingtian Zhang, et al. "S3: a scalable in-memory skip-list index for key-value store", VLDB 2019
  - Sprenger, et al. "Cache-Sensitive Skip List: Efficient Range Queries on Modern CPUs", Data Management on New Hardware 2016 [:octocat:](https://github.com/flippingbits/cssl.git)
  - Hokeun Cha, et al. "Blink-hash: An Adaptive Hybrid Index for In-Memory Time-Series Databases", VLDB 2023
  - Hongbo Kang, et al. "PIM-Tree: A Skew-Resistant Index for Processing-in-Memory", VLDB 2022
  - Ajit mathew, et al. "HydraList: a scalable in-memory index using asynchronous updates and partial replication", VLDB 2020
  - Wenlong Ma, et al. "BiloKey: A Scalable Bi-Index Locality-Aware In-Memory Key-Value Store", IEEE TPDS 2019
- Survey
  - Z. Xie, et al. "A Comprehensive Performance Evaluation of Modern In-Memory Indices", ICDE 2018
  - Abdullah Talha Kabakus, et al, "A performance evaluation of in-memory databases", J. King Saud Univ. Comput. Inf. Sci. 2017
  - Venkata Sai Pavan Kumar Vadrevu et al, "Tutorial: The Ubiquitous Skiplist, its Variants, and Applications in Modern Big Data Systems"

  

### Learned Index
#### Read-Only Learned Index
- Maltry, Marcel, et al. "A critical analysis of recursive model indexes.", VLDB 22 [:octocat:](https://github.com/BigDataAnalyticsGroup/analysis-rmi)
- Ferragina, Paolo, et al. "The PGM-index: a fully-dynamic compressed learned index with provable worst-case bounds.", VLDB 20 [:octocat:](https://gitub.com/gvinciguerra/PGM-index) [:bar_chart:](https://pgm.di.unipi.it/)
- Kipf, Andreas, et al. "RadixSpline: a single-pass learned index.", aiDM@SIGMOD 20[:octocat:](https://github.com/learnedsystems/RadixSpline) [:clapper:](https://youtu.be/or0JXc4UQ-4?si=onilmCv3VKvoB_b5)
- Marcus, Ryan, et al. **"Benchmarking learned indexes."**, VLDB 20 [:octocat:](https://github.com/learnedsystems/SOSD)
- Minguk, Choi, et al. **"Can Learned Indexes be Build-Efficient? A Deep Dive into Sampling Trade-Offs."**, SIGMOD 24 [:octocat:](https://github.com/DKU-StarLab/Benchmark4Sampling)


#### Updatable Learned Index
- Ding, Jialin, et al. "ALEX: an updatable adaptive learned index.", SIGMOD 20 [:clapper:](https://youtu.be/wVxbOcwYZ8I?si=Aw4cnegvYFVEAE4c) [:octocat:](https://github.com/microsoft/ALEX.git)
- Wu, Jiacheng, et al. "Updatable learned index with precise positions.", VLDB 21 [:clapper:](https://youtu.be/cUhpkA7LbgA?si=FOoRZNqyDkFEgc3E) [:octocat:](https://github.com/Jiacheng-WU/lipp.git)
- Wongkham, Chaichon, et al. "**Are updatable learned indexes ready?**", VLDB 22' [:octocat:](https://github.com/gre4index/GRE)
- Sun, Zhaoyan, et al. **"Learned Index: A Comprehensive Experimental Evaluation."** VLDB 23.
- Ge, Jiake, et al. **"SALI: A Scalable Adaptive Learned Index Framework based on Probability Models."**, SIGMOD 24 [:octocat:](https://github.com/cds-ruc/SALI/tree/a7eee3449e07b5b0d4f34507311fbf2224523c8d)


#### Algorithm & Application
- Error-Bounded PLA Model
  - Xie, Qing, et al. **"Maximum error-bounded piecewise linear representation for online stream approximation."** VLDB journal 14 [:octocat:](https://github.com/RyanMarcus/plr.git)
- Key-Value Store
  - Dai, Yifan, et al. "From {WiscKey} to Bourbon: A Learned Index for {Log-Structured} Merge Trees.", OSDI 20 [:octocat:](https://bitbucket.org/daiyifandanny/learned-leveldb/src/master/)
  - Yu, Geoffrey X., et al. "Treeline: an update-in-place key-value store for modern storage.", VLDB 22 [:octocat:](https://github.com/mitdbg/treeline) [:bar_chart:](https://people.csail.mit.edu/markakis/presentations/2023-08-31_VLDB_TreeLine_Presentation.pdf)
- NVM Device
  - Lu, Baotong, et al. "APEX: A high-performance learned index on persistent memory.", VLDB 21 [:octocat:](https://github.com/baotonglu/apex.git)
  - Ge, Jiake, et al. "Cutting Learned Index into Pieces: An In-depth Inquiry into Updatable Learned Indexes." ICDE 23.
- FTL
  - Sun, Jinghan, et al. **"Leaftl: A learning-based flash translation layer for solid-state drives."**, ASPLOS 23 [:octocat:](https://github.com/platformxlab/LeaFTL.git)

#### Extensive ML4System Paper List
  - LumingSun, ["ML4DB-paper-list"](https://github.com/LumingSun/ML4DB-paper-list)

### Lecture
  - [CMU, "Intro to Database Systems", Fall 2023](https://youtube.com/playlist?list=PLSE8ODhjZXjbj8BMuIrRcacnQh20hmY9g&si=vIqTjyEuCJWWfprn)
    - This course is about the design/implementation of DBMS, not about "how to use a DBMS".
    - It is recommended to understand indexes in the overall flow of DBMS. **Be sure to take courses 7, 8, and 9**.
  - [Tim Kraska, "AWS On Air ft. How will AI revolutionize databases?", 2023](https://youtu.be/zyRmXFj_ej4?si=UdfpqIeCJaos0R0W)
  - [Jongmoo Choi,"Key-Value Store: Database for Unstructured Bigdata (KOR)",  2021](https://mooc.dankook.ac.kr/courses/61d537a3b6b71841651153b3) [:bar_chart:](https://github.com/DKU-StarLab/leveldb-study/blob/761b550973ab6d1e88189190e66c0ee19a52aa12/introduction/Jongmoo%20Choi,%20Key-Value%20Store%20-%20Database%20for%20Unstructured%20Bigdata,%202021.pdf)
  - [MIT, "Machine Learning for Systems", 2021](https://dsg.csail.mit.edu/6.887/sched.php)

### For Beginners
  - Lectures
    - [SNU 쓰디연구소, JTJ의 리눅스탐험 (linux, makefile, vim, gdb)](https://youtube.com/playlist?list=PL0vWyY_q7XP_JMzDKVbOc3aXEEDPjYTUX&si=O8SHNAuP1eD8tShn)
    - [따라하면서 배우는 Shell Programming](https://youtube.com/playlist?list=PLApuRlvrZKog2XlvGJQh9KY8ePCvUG7Je&si=kfY4Uw9oPrRjskCo)
    - [Matplotlib 단기집중과정](https://youtu.be/3Xc3CA655Y4?si=7vqUTosyHWppuADv)
    - [제대로 파는 Git & GitHub - 깃 끝.장.내.기](https://youtu.be/1I3hMwQU6GU?si=fW8B-39g8SR4X_Sv)
  
  - Documents
    - [권창현, "박사과정 학생이 유의해야 하는 점"](https://thoughts.chkwon.net/phd-student-professor-faq/)
    - [문수복, "개별연구/졸업연구를 고민하는 학생들을 위한 간추린 자료"](https://sbmoon.tistory.com/245)
    - [문수복, "논문 제 1 저자의 책임"](https://sbmoon.tistory.com/253)  
    - [S. Keshav, "How to Read a Paper"](https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf)
    - [Remzi Arpaci-Dusseau, "Graduate School: Keys To Success"](https://youtu.be/fqPSnjewkuA?si=adHJlDhKV06bmdrH)
    - [Remzi Arpaci-Dusseau, "25 Years of Storage Research and Education: A Retrospective"](https://youtu.be/u9RECEzxk6I?si=yA7FVDKOD0RzVlGi)

* Tools
  - [GDB](https://www.sourceware.org/gdb/)
  - [Understand](https://licensing.scitools.com/download) 
  - [Uftrace](https://github.com/namhyung/uftrace)

* File
  - [presentation file format](./presentation_file/presentation_file_format.pptx)
  - [kcc research paper format](./file/%5Bformat%5Dresearch_paper(KCC).hwp)

* Previous Study
  - [DKU Leveldb Study, 2022](https://github.com/DKU-StarLab/leveldb-study)
  - [DKU RocksDB Festival, 2021](https://github.com/DKU-StarLab/RocksDB_Festival)

## Members
* Student: [Suhwan Shin](https://github.com/Student5421), [Zhu Yongjie](https://github.com/arashio1111), Boseung Kim, Yeojin Oh, Nakyeong Kim, Yeongyu Choi 
* Assistant: [Hojin Shin](https://github.com/shinhojin), [Minguk Choi](https://github.com/min-guk)
* Professor: [Jongmoo Choi](http://embedded.dankook.ac.kr/~choijm/)

## Schedule
* Date: Every Wensday in January, February
* Time: 14:00 ~ 16:00
* Place: Dankook University Software ICT Hall Room 507
