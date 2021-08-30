About r-doc2vec
===============

Home: https://github.com/bnosac/doc2vec

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/r-doc2vec-feedstock/blob/master/LICENSE.txt)

Summary: Learn vector representations of sentences, paragraphs or documents by using the 'Paragraph Vector' algorithms, namely the distributed bag of words ('PV-DBOW') and the distributed memory ('PV-DM') model. The techniques in the package are detailed in the paper "Distributed Representations of Sentences and Documents" by Mikolov et al. (2014), available at <arXiv:1405.4053>. The package also provides an implementation to cluster documents based on these embedding using a technique called top2vec. Top2vec finds clusters in text documents by combining techniques to embed documents and words and density-based clustering. It does this by embedding documents in the semantic space as defined by the 'doc2vec' algorithm. Next it maps these document embeddings to a lower-dimensional space using the 'Uniform Manifold Approximation and Projection' (UMAP) clustering algorithm and finds dense areas in that space using a 'Hierarchical Density-Based Clustering' technique (HDBSCAN). These dense areas are the topic clusters which can be represented by the corresponding topic vector which is an aggregate of the document embeddings of the documents which are part of that topic cluster. In the same semantic space similar words can be found which are representative of the topic. More details can be found in the paper 'Top2Vec: Distributed Representations of Topics' by D. Angelov available at <arXiv:2008.09470>.

Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64_r_base4.0</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master&jobName=linux&configuration=linux_64_r_base4.0" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_64_r_base4.1</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master&jobName=linux&configuration=linux_64_r_base4.1" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_r_base4.0</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master&jobName=osx&configuration=osx_64_r_base4.0" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64_r_base4.1</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master&jobName=osx&configuration=osx_64_r_base4.1" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_r_base4.0</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master&jobName=win&configuration=win_64_r_base4.0" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64_r_base4.1</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=13747&branchName=master">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/r-doc2vec-feedstock?branchName=master&jobName=win&configuration=win_64_r_base4.1" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--doc2vec-green.svg)](https://anaconda.org/conda-forge/r-doc2vec) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-doc2vec.svg)](https://anaconda.org/conda-forge/r-doc2vec) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-doc2vec.svg)](https://anaconda.org/conda-forge/r-doc2vec) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-doc2vec.svg)](https://anaconda.org/conda-forge/r-doc2vec) |

Installing r-doc2vec
====================

Installing `r-doc2vec` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `r-doc2vec` can be installed with:

```
conda install r-doc2vec
```

It is possible to list all of the versions of `r-doc2vec` available on your platform with:

```
conda search r-doc2vec --channel conda-forge
```


About conda-forge
=================

[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.com/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-doc2vec-feedstock
============================

If you would like to improve the r-doc2vec recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-doc2vec-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@conda-forge/r](https://github.com/conda-forge/r/)

