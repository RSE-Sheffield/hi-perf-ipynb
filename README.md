# An introduction to high-performance Python using Jupyter

[Will Furnass][wf], University of Sheffield's [Research Software Engineering][uos-rse] team, 2018.

A brief guide to parallel programming using Python and the [Jupyter Notebook][jupyter].

## Aims

The main aim is to equip the researcher who already has some knowledge of the Python scientific computing stack with
an understanding of relevant conceptual approaches to parallel programming and of practical approaches to realising those concepts using popular Python packages.

A secondary aim is to demonstrate the potential of [JupyterHub on Grid Engine][jh-on-sharc] computer clusters
as a high-performance Python programming environment for those with limited knowledge of Linux and the Unix shell. 
JupyterHub has been deployed on the University of Sheffield's [ShARC][jh-on-sharc] cluster using 
funding from the OpenDreamKit project (see [Acknowledgements](#Acknowledgements)).
This teaching material was designed to be used on ShARC but is also relevant to other environments where Jupyter and sufficient hardware resources are available.

## Learning outcomes

* Understanding of why parallelisation is of increasing performance given the death of Moore's Law
* Understanding of the different types of parallelism and their merits
* Basic understanding of theoretical speedups and Amdahl's Law
* Understaning of communication vs computation costs
* Ability to identify and use libraries that can distribute non-Python work between threads
* Ability to distribute Python work between processes using `multiprocessing`

## Lessons

1. [Parallelisation using packages that support multithreading](multithreading.ipynb)
1. [Parallelising your own code using multiple Python processes on a single machine](multiprocessing.ipynb)

## Further reading

* Wilkinson, B. and Allen, M. (1999). *Parallel programming: techniques and applications using networked workstations and parallel computers*. 
  Prentice Hall, Upper Saddle River, N.J. ISBN: 0-13-671710-1
* Gorelick, M. and Ozsvald, I. (2014). *High performance Python*, 
  First edition. ed. O’Reilly, Sebastopol, CA.  ISBN: 978-1-4493-6159-4
* [Using JupyterHub on the University of Sheffield's ShARC cluster](http://docs.hpc.shef.ac.uk/en/latest/hpc/jupyterhub.html)

## Acknowledgements

The development of this material was funded by [OpenDreamKit][odk], 
a [Horizon2020][h2020] European [Research Infrastructure][res-inf] project ([676541][odk-grant]) that aims to 
advance the open source computational mathematics ecosystem.

<div align="center"> 
<img src="static/opendreamkit.svg" alt="OpenDreamKit logo" alt="LabCollector logo" width="30%" />
</div>

[odk]: http://opendreamkit.org/
[h2020]: https://ec.europa.eu/programmes/horizon2020/
[res-inf]: https://ec.europa.eu/programmes/horizon2020/en/h2020-section/european-research-infrastructures-including-e-infrastructures
[odk-grant]: http://cordis.europa.eu/project/rcn/198334_en.html
[uos-rse]: http://rse.shef.ac.uk
[wf]: http://learningpatterns.me
[jh-on-sharc]: http://docs.hpc.shef.ac.uk/en/latest/hpc/jupyterhub.html
[jupyter]: http://jupyter.org/
