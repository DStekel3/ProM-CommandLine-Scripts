# ProM-CommandLine-Scripts
This repository is a collection of ProM scripts, which is a command-line approach for applying plugins in ProM.

For more information on using ProM through a command-line, I refer you to https://dirksmetric.wordpress.com/2015/03/11/tutorial-automating-process-mining-with-proms-command-line-interface/.

It could happen that you run into a "java.lang.OutOfMemoryError: GC overhead limit exceeded" exception.
This happens when the Garbage Collector of JVM is too busy with removing garbage, because the heap generation is at its limit.

Although it is not the best solution, an easy fix would be to adjust the -Xmx -XX:MaxPermSize= parameters. For instance, set these parameters to -Xmx4G -XX:MaxPermSize=2G. This will give your program more memory space, such that the exception occurs less frequently.
