BigCloneBench
=============

BigCloneBench is a clone detection benchmark of known clones in the IJaDataset source repository.  The current version of the benchmark, IJaDataset (with modifications), and tools for measuring clone detection recall are available below.

Upcoming
========
We are currently working on a version with a significantly larger variety of clones (in terms of cloned functionalities).  Please look forward to this!  For now use the ERA Download "New Version" below.

ERA Download (New Version)
==========================
This is an updated version of the ERA release.  There are some minor changes to the database and IJaDataset to improve the quality of measured recall.  We have also released evaluation tools for measuring recall based on our work in [2].

[BigCloneBench Database](https://drive.google.com/file/d/0B70GNOiQD-X7aDNaR2lwQ1NGeUk/view?usp=sharing):
This is the benchmark database.
    
[IJaDataset 2.0 + BigCloneBench Samples](https://drive.google.com/file/d/0B70GNOiQD-X7a2xRbGtXLXkxT1E/view?usp=sharing):
This is the full IJaDataset - inter-project java source-code dataset, including modifications for BigCloneBench.
    
[IJaDataset 2.0 - BigCloneBench Reduced Version](https://drive.google.com/file/d/0B70GNOiQD-X7b1lCRDBKakt6Tnc/view?usp=sharing):
Most tools do not scale well to IJaDataset.  This version reduces the number of source files to only those which contain known true or false clones of the functionalities tagged in BigCloneBench.  This contains a folder per functionality with the source files containing tagged functions.  This reduces/removes the scalability challenge when measuring recall.  See instructions provided in the "Clone Deteciton Recall Tools" distributable for more details/suggestions.
    
[Clone Detection Recall Tools](https://github.com/jeffsvajlenko/BigCloneBenchEval):
A collection of tools for measuring clone detection recall using the benchmark.  Based on the clone-deteciton experiment in [2].  Tools and instructions are kept in the linked github repository.  Clone the repository to get the latest version, and use git pull to update.

If you have any questions about this release, using the tools, or measuring recall, please contact us and we will be happy to assist.

ERA Download (Old Version)
==========================
This is a peer reviewed version of the benchmark, as described in our ICSME'14 ERA paper.  You should prefer to use the new version above, which is compatible with the clone detector evaluation tools.

[BigCloneBench Database](https://drive.google.com/file/d/0B70GNOiQD-X7RnYzY3g5WEp3WlE/view?usp=sharing)

[IJaDataset 2.0 + BigCloneBench Samples](https://drive.google.com/file/d/0B70GNOiQD-X7ZDVBMzRUWktDUWs/view?usp=sharing)

License
=======
Benchmark: The benchmark is distributed under the Creative Commons, Attribution-NonCommercial-NoDerivatives.  This license includes the benchmark database and its derivatives.  For attribution, please cite this page, and our publications below.  This data is provided free of charge for non-commercial and academic benchmarking and experimentation use.  If you would like to contribute to the benchmark, please contact us.  If you believe you intended usage may be restricted by the license, please contact us and we can discuss the possibilities.

IJaDataset: We distribute here IJaDataset 2.0 with additions and modifications for the benchmark.  The files contained within were crawled from open-source projects.  Their in-file licenses are maintained as-is.  Additionally, the benchmark database lists the source of each file, and their detected licensing.  IJaDataset 2.0 is from the SECold Project: http://www.secold.org/projects/seclone.

Publications
============

[1] Jeffrey Svajlenko, Judith F. Islam, Iman Keivanloo, Chanchal K. Roy and Mohammad Mamun Mia, "Towards a Big Data Curated Benchmark of Inter-Project Code Clones", In Proceedings of the Early Research Achievements track of the 30th International Conference on Software Maintenance and Evolution (ICSME 2014), 5 pp., Victoria, Canada,  September 2014.

[2] Jeffrey Svajlenko and Chanchal K. Roy, “Evaluating Clone Detection Tools with BigCloneBench”, In Proceedings of the 31st International Conference on Software Maintenance and Evolution (ICSME 2015), 10 pp., Bremen, Germany, September 2015.

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
