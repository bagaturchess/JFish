![JFish logo](JFish.jpg)

# Overview

This version of the Bagatur chess engine integrates the powerful NNUE network and inference technology from the well-known Stockfish engine.
It leverages NNUE through JNI, while the rest of the implementation is based on the Bagatur engine's original Java code.
As of 2024, it aims to be the strongest Java-based chess engine in the world.

If you appreciate this project, consider giving it a star! :-)

# Downloads for desktop computer

Downloads could be found as a standard github release <a href="https://github.com/bagaturchess/JFish/releases">here</a>.

# Running it

* **Windows**, there are *.exe files for direct run as well as bat files. Here are the steps necessary to run the engine:
  * Download an arbitrary UCI user interface. For example the most popular one is <a href="http://www.playwitharena.com/">Arena Chess GUI</a>.
  * Install the UCI user interface on your computer.
  * Ensure that the Java Runtime Environment (JRE) 1.8 or later is installed on your computer (it should be the case nowadays but if not, have in mind that JRE is required, only JDK doesn't work). It could be downloaded from <a href="https://java.com/">java.com</a>
  * Unpack this distribution somewhere (Arena has a sub-folder called 'engines', you can extract it there).
  * Open the UCI user interface and register the engine inside (You should become familiar with the installed UCI user interface anyway).
  * E2-E4 and enjoy :-)
* **Linux**, still not supported.

# UCI Options

See [Bagatur UCI options](https://github.com/bagaturchess/Bagatur#UCI-Options)

# Syzygy Endgame Tablebases

The download of JFish contains subset of syzygy tablebases placed under ./data/egtb/ directory. It contaiuns 22 of the most common endgames with up to 5 pieces. By default the option 'SyzygyPath' is set to this directory. You could change this UCI option if you have complete or bigger set of syzygy tablebases downloaded on your computer.

# Elo Rating

The Elo rating of JFish is +160 Elo over the standard Bagatur engine version 5.1b, which means JFish has around 3550 Elo.

# Source code

This repository contains only the binaries under the release section.
If you need the sources please refer to the <a href="https://github.com/bagaturchess/Bagatur">Bagatur Chess Engine</a>.
JFish is actually a compilation of Bagatur with different flavour/configuration.
The different code is for the integration with Stockfish NNUE and could be found
<a href="https://github.com/bagaturchess/Bagatur/tree/master/NNUE/src/bagaturchess/nnue_v5">here</a>
and <a href="https://github.com/bagaturchess/Bagatur/tree/master/LearningImpl/src/bagaturchess/deeplearning/impl_nnue_v2b">here</a>.

# Contact the Author

In order to contact me, you could use LinkedIn <a href="https://www.linkedin.com/in/topchiyski/">Krasimir Topchiyski</a> or email me at k_topchiyski@yahoo.com

# Credits

1. https://github.com/bagaturchess/Bagatur which is used for all the Java code except NNUE.
2. Stockfish team for the great chess engine.
3. https://github.com/VedantJoshi1409/stockfish_nnue_probe which is used as a basis (with some modifications) for the compilation of the StockfishNNUE.dll

