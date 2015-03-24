# Volt
Pure java NGS mapping soft run on Hadoop 2.0
Volt is pure JAVA Next Generation Sequence (NGS) mapping soft that run both on Hadoop
and standalone environment. 
The accuracy is comparable to BWA-MEM and novoalign with speed faster than those aligner.
Volt use mulththread mapper that enable optimized processing under multicore processor and 
Hadoop YARN environment. It use about 5GB of RAM to hold human reference and require
additional 2-5GB to run. In Hadoop mode, Volt reads file from HDFS and write BAM 
file usng Hadoop-BAM api where reads sorting is done using Hadoop in build function. 
With Pure Java architecture Volt was directory integrated into Hadoop, 
so there is no IO bottleneck by using Hadoop streaming, nor additional
setting for reads mapper is not necessary other than running Hadoop job.
Currently, Volt support BAM format for output.
