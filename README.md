<a href="https://milvus.io/hacktoberfest-2021">
    <img src="https://zilliz-cms.s3.us-west-2.amazonaws.com/milvus_hacktoberfest_15ba8e5083.jpeg" alt="Join Hacktoberfest with Milvus">
</a>

# Milvus Python SDK

[![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
[![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
[![Downloads](https://pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
[![Downloads](https://pepy.tech/badge/pymilvus/month)](https://pepy.tech/project/pymilvus/month)
[![Downloads](https://pepy.tech/badge/pymilvus/week)](https://pepy.tech/project/pymilvus/week)
[![license](https://img.shields.io/hexpm/l/plug.svg?color=green)](https://github.com/milvus-io/pymilvus/blob/master/LICENSE)
[![Mergify Status][mergify-status]][mergify]


Python SDK for [Milvus](https://github.com/milvus-io/milvus). To contribute code to this project, please read our [contribution guidelines](https://github.com/milvus-io/milvus/blob/master/CONTRIBUTING.md) first. If you have some ideas or encounter a problem, you can find us in the Slack channel [#py-milvus](https://milvusio.slack.com/archives/C024XTWMT4L).


## Compatibility
The following collection shows Milvus versions and recommended PyMilvus versions:

|Milvus version| Recommended PyMilvus version |
|:-----:|:-----:|
| 1.0.* | 1.0.1 |
| 1.1.* | 1.1.2 |
| 2.0.0-RC7 | 2.0.0rc7 |
| 2.0.0-RC8 | 2.0.0rc8 |


## Installation

You can install PyMilvus via `pip` or `pip3` for Python 3.6+:

```shell
$ pip3 install pymilvus
```

You can install a specific version of PyMilvus by:

```shell
$ pip3 install pymilvus==2.0.0rc8
```

You can upgrade PyMilvus to the latest version by:

```shell
$ pip3 install --upgrade pymilvus
```


## Documentation

Documentation is available online: https://milvus.io/api-reference/pymilvus/v2.0.0rc8/install.html.


## Packages

### Released packages

The release of PyMilvus is managed on GitHub, and GitHub Actions will package and upload each version to PyPI.

The release version number of PyMilvus follows PEP440, the format is x.y.z, and the corresponding git tag name is vx.y.z (x/y/z are numbers from 0 to 9).

For example, after PyMilvus 1.0.1 is released, a tag named v1.0.1 can be found on GitHub, and a package with version 1.0.1 can be downloaded on PyPI.

### Developing packages

The commits on the development branch of each version will be packaged and uploaded to Test PyPI.
Development branches refer to branches such as 1.0 and 1.1, and version releases are generated from the development branches, such as 1.0.1 and 1.0.2.

The package name generated by the development branch is x.y.z.dev<dist>, where <dist> is the number of commits that differ from the most recent release.

For example, after the release of 1.0.1, two commits were submitted on the 1.0 branch. At this time, the automatic packaging version number of the development branch is 1.0.1.dev2.

To install the package on test.pypi.org, you need to append the parameter --index-url after pip, for example:
```shell
$ python3 -m pip install --index-url https://test.pypi.org/simple/ pymilvus
```


## License
[Apache License 2.0](LICENSE)


[mergify]: https://mergify.io
[mergify-status]: https://img.shields.io/endpoint.svg?url=https://gh.mergify.io/badges/milvus-io/pymilvus&style=plastic
