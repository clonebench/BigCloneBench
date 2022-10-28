BigCloneBench
=============

BigCloneBench is a clone detection benchmark of known clones in the IJaDataset source repository.  The current version of the benchmark, IJaDataset (with modifications), and tools for measuring clone detection recall are available below.

Derivative works using the benchmark should cite [1], while works using the recall measurement process should also cite [2] and [3].

BigCloneEval
============
We have now released BigCloneEval, a framework for evaluating clone detection tools with BigCloneBench.  It is very easy to use, and comes with optimized versions of BigCloneBench and IJaDatset for evaluating clone detection tools.  You can use this version if you simply want to measure the recall of your clone detection tool.  Use the full BigCloneBench database if you want to implemetn a custom experiment over the data.

BigCloneEval can be found [here](http://jeffsvajlenko.weebly.com/bigcloneeval.html).

BigCloneBench Version 2 (**Use This Version**)
==========================================

The latest BigCloneBench is distributed with BigCloneEval [here](https://github.com/jeffsvajlenko/BigCloneEval).  It is significantly larger than the ERA version, and is distributed as a h2database file with a much simpler schema.  If you need the full BigCloneBench, with all the validation artifacts, please contact us and we can arrange to send you a copy (it is quite large).

IJaDataset with the expanded files is available here: [IJaDataset 2.0 + BigCloneBench Samples](https://1drv.ms/u/s!AhXbM6MKt_yLj_tk29GJnc9BKoIvCg?e=oVTVJm).

BigCloneBench full database (postgresql) is available here: [BigCloneBench_Postgresql](https://1drv.ms/u/s!AhXbM6MKt_yLj_tmo-UxK2QTwMk2ew?e=YF9w0g).

Limits on OneDrive means for these large files it may be necissary to login before the files can be downloaded.

ERA (Outdated) 
=============

** This version is out of date.  I reccomend using the 2nd version included with BigCloneEval for a much larger dataset. **

This is an updated version of the ERA release.  There are some minor changes to the database and IJaDataset to improve the quality of measured recall.  We have also released evaluation tools for measuring recall based on our work in [2].

[BigCloneBench Database](https://1drv.ms/u/s!AhXbM6MKt_yLj_Nv7H-8OoPD45lWeg?e=5yORQL):
This is the benchmark database.
    
[IJaDataset 2.0 + BigCloneBench Samples](https://1drv.ms/u/s!AhXbM6MKt_yLj_N3FAIGw3CJb1JGOg?e=NsP59Z):
This is the full IJaDataset - inter-project java source-code dataset, including modifications for BigCloneBench.
    
[IJaDataset 2.0 - BigCloneBench Reduced Version](https://1drv.ms/u/s!AhXbM6MKt_yLj_Nsc798DA-UJ4DFew?e=fp157L):
Most tools do not scale well to IJaDataset.  This version reduces the number of source files to only those which contain known true or false clones of the functionalities tagged in BigCloneBench.  This contains a folder per functionality with the source files containing tagged functions.  This reduces/removes the scalability challenge when measuring recall.  See instructions provided in the "Clone Deteciton Recall Tools" distributable for more details/suggestions.

ERA Version 1 (Outdated)
==========================

** This version is out of date.  I reccomend using the 2nd version included with BigCloneEval for a much larger dataset. **

This is a peer reviewed version of the benchmark, as described in our ICSME'14 ERA paper.  You should prefer to use the new version above, which is compatible with the clone detector evaluation tools.

[BigCloneBench Database](https://1drv.ms/u/s!AhXbM6MKt_yLj_N9oMHZox6lUM7xqw?e=XVWQ4S)

[IJaDataset 2.0 + BigCloneBench Samples](https://1drv.ms/u/s!AhXbM6MKt_yLj_N80wvpc_ag9NJobg?e=kzf4eN)

License
=======
Benchmark: The benchmark is distributed under the Creative Commons, Attribution-NonCommercial-NoDerivatives.  This license includes the benchmark database and its derivatives.  For attribution, please cite this page, and our publications below.  This data is provided free of charge for non-commercial and academic benchmarking and experimentation use.  If you would like to contribute to the benchmark, please contact us.  If you believe you intended usage may be restricted by the license, please contact us and we can discuss the possibilities.

IJaDataset: We distribute here IJaDataset 2.0 with additions and modifications for the benchmark.  The files contained within were crawled from open-source projects.  Their in-file licenses are maintained as-is.  Additionally, the benchmark database lists the source of each file, and their detected licensing.  IJaDataset 2.0 is from the SECold Project: http://www.secold.org/projects/seclone.

Publications
============

[1] Jeffrey Svajlenko, Judith F. Islam, Iman Keivanloo, Chanchal K. Roy and Mohammad Mamun Mia, "Towards a Big Data Curated Benchmark of Inter-Project Code Clones", In Proceedings of the Early Research Achievements track of the 30th International Conference on Software Maintenance and Evolution (ICSME 2014), 5 pp., Victoria, Canada,  September 2014.

[2] Jeffrey Svajlenko and Chanchal K. Roy, “Evaluating Clone Detection Tools with BigCloneBench”, In Proceedings of the 31st International Conference on Software Maintenance and Evolution (ICSME 2015), 10 pp., Bremen, Germany, September 2015.

[3] Jeffrey Svjalenko and Chanchal K. Roy, "BigCloneEval: A Clone Detection Tool Evaluation Framework with BigCloneBench", In Proceedigns of the 32nd International Conference on Software Maintence and Evolution (ICSME 2016), to appear.

Contact
=======
Benchmark Maintainer: Jeffrey Svajlenko: jeff.svajlenko@gmail.com

Judith F. Islam: judithfran@gmail.com

Iman Keivanloo: iman.keivanloo@queensu.ca

Chanchal K. Roy: chanchal.roy@usask.ca


Acknowledgements
================
The following people have provided clone oracling efforts (in no particular order):
- Judith F. Islam
- Mohammad Mamun Mia
- Graeme Daly
- Jeffrey Svajlenko
- Chanchal Roy
- Muhammad Asaduzzamn
- Shamima Yeasmin
- Manishankar Mondal
- Mike Hoffert
