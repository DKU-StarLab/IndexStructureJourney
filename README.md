# IndexStructureJourney

2024 [DKU System Software Lab](https://sslab.dankook.ac.kr/) Index  Study

## Goals
* Study and Analyze Index Structures
* Write document.
* (Optional) Write a research paper on what you learned.


### Paper List
#### Traditional Index
- B+Tree
- SkipList
- ART
- MassTree
- LSM-Tree

#### Read-Only Learned Index
- Maltry, Marcel, et al. "A critical analysis of recursive model indexes.", VLDB 22' [:octocat:](https://github.com/BigDataAnalyticsGroup/analysis-rmi)
- Ferragina, Paolo, et al. "The PGM-index: a fully-dynamic compressed learned index with provable worst-case bounds.", VLDB 20' [:octocat:](https://gitub.com/gvinciguerra/PGM-index)
- Kipf, Andreas, et al. "RadixSpline: a single-pass learned index.", aiDM@SIGMOD 20[:octocat:](https://github.com/learnedsystems/RadixSpline) [:clapper:](https://youtu.be/or0JXc4UQ-4?si=onilmCv3VKvoB_b5)
- Marcus, Ryan, et al. "Benchmarking learned indexes.", VLDB 20 [:octocat:](https://github.com/learnedsystems/SOSD)
- Minguk, Choi, et al. "Can Learned Indexes be Build-Efficient? A Deep Dive into Sampling Trade-Offs.", SIGMOD


#### Updatable Learned Index
- Ding, Jialin, et al. "ALEX: an updatable adaptive learned index.", SIGMOD 20 [:clapper:](https://youtu.be/wVxbOcwYZ8I?si=Aw4cnegvYFVEAE4c)
- Wu, Jiacheng, et al. "Updatable learned index with precise positions.", VLDB 21
- Ge, Jiake, et al. "SALI: A Scalable Adaptive Learned Index Framework based on Probability Models.", SIGMOD 23
- Wongkham, Chaichon, et al. "Are updatable learned indexes ready?.", VLDB 22' [:octocat:](https://github.com/gre4index/GRE)

#### Application
- Key-Value Store
  - Dai, Yifan, et al. "From {WiscKey} to Bourbon: A Learned Index for {Log-Structured} Merge Trees.", OSDI 20 [:octocat:](https://bitbucket.org/daiyifandanny/learned-leveldb/src/master/)
  - Yu, Geoffrey X., et al. "Treeline: an update-in-place key-value store for modern storage.", VLDB 22 [:octocat:](https://github.com/mitdbg/treeline) [:bar_chart:](https://people.csail.mit.edu/markakis/presentations/2023-08-31_VLDB_TreeLine_Presentation.pdf)
- NVM Device
  - Lu, Baotong, et al. "APEX: A high-performance learned index on persistent memory.", VLDB 21
- FTL
  - Sun, Jinghan, et al. "Leaftl: A learning-based flash translation layer for solid-state drives.", ASPLOS 23

### References
* Lecture
  - [CMU Intro to Database Systems , Fall 2023)](https://youtube.com/playlist?list=PLSE8ODhjZXjbj8BMuIrRcacnQh20hmY9g&si=vIqTjyEuCJWWfprn)
  - [Tim Kraska, 『AWS On Air ft. How will AI revolutionize databases?』, 2023](https://youtu.be/zyRmXFj_ej4?si=UdfpqIeCJaos0R0W)
  - [Jongmoo Choi, 『Key-Value Store: Database for Unstructured Bigdata (KOR)』,  2021](https://mooc.dankook.ac.kr/courses/61d537a3b6b71841651153b3)

  
* Documents
  - [MIT, "Machine Learning for Systems", 2021](https://dsg.csail.mit.edu/6.887/sched.php)
  - [Jongmoo Choi,"Key-Value Store: Database for Unstructured Bigdata", 2021](https://github.com/DKU-StarLab/leveldb-study/blob/761b550973ab6d1e88189190e66c0ee19a52aa12/introduction/Jongmoo%20Choi,%20Key-Value%20Store%20-%20Database%20for%20Unstructured%20Bigdata,%202021.pdf)


* Previous Study
  - [DKU Leveldb Study, 2022]()
  - [DKU RocksDB Festival, 2021](https://github.com/DKU-StarLab/RocksDB_Festival)

### For Beginners
  - Lectures
    - [JTJ의 리눅스탐험](https://youtube.com/playlist?list=PL0vWyY_q7XP_JMzDKVbOc3aXEEDPjYTUX&si=O8SHNAuP1eD8tShn)
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
  - [presentation format](./file/%5Bformat%5Dleveldb_study_ppt.pptx)
  - [kcc research paper format](./file/%5Bformat%5Dresearch_paper(KCC).hwp)


## Members
* Student: [Suhwan Shin](https://github.com/Student5421), [Zhu Yongjie](https://github.com/arashio1111), Boseung Kim, Yeojin Oh, 김나경, 이지수, 최연규 
* Assistant: [Hojin Shin](), [Minguk Choi](https://github.com/min-guk), [Zhao Guangxun](https://github.com/ErosBryant)
* Professor: [Jongmoo Choi](http://embedded.dankook.ac.kr/~choijm/)

## Schedule
* Date: Every Wensday in January, February
* Time: 14:00 ~ 16:00
* Place: Dankook University Software ICT Hall Room 507