# Noble

Daniel Standage, 2018  
https://osf.io/anr56/

[![Docker image status at quay.io](https://quay.io/repository/standbio/noble/status "Docker ready")](https://quay.io/repository/standage/noble)

**Noble** is a collection of data sets for evaluating and benchmarking *de novo* variant discovery methods.
You can freely and anonymously download files containing the associated simulated genetic data under the terms of the CC BY 4.0 license: see [DATALICENSE.txt](doc/DATALICENSE.txt) for details.
You are also free to use, copy, modify, and distribute source code from this project with attribution under the terms of the MIT license: see [CODELICENSE.txt](doc/CODELICENSE.txt) for details.

Scientific ethics dictate that you credit this resource if you use it in any research publication: see [CITATION.md](doc/CITATION.md) for more details.


## How do I use Noble?

<details>
    <summary>I want to use the data to benchmark my new method.</summary>

All of the data files are stored on Amazon S3 and can be downloaded from your web browser or (preferably) using shell tools like `wget` or `curl`.
See [DOWNLOADS.md](doc/DOWNLOADS.md) for more details.

</details>
<details>
    <summary>I want to recreate the data sets from scratch.</summary>

The [build/](build/) directory contains information on the workflow used to create the data files, instructions on how to invoke the workflow, and a description of the software prerequisites and configuration.

</details>
<details>
    <summary>I want to reproduce a published analysis.</summary>

The [eval/](eval/) directory contains details on our accuracy assessment of [kevlar](https://kevlar.readthedocs.io) on Noble.

</details>
<details>
    <summary>I want borrow code from this project and create my own.</summary>

You are free to create a fork of this project and adapt it for your own needs, as long as you attribute the original work.

</details>
<details>
    <summary>I'm having trouble with Noble.</summary>

Please use the [GitHub tracker](https://github.com/StandBio/noble/issues) to report bugs or submit support requests.

</details>
