<p align="center"><img src="https://github.com/Nefcore/CRLFsuite/blob/main/static/crlfsuite_logo.png" height="200"/></p>
<h2 align="center">CRLFsuite</h2>

CRLFsuite is a fast tool specially degined to scan `CRLF injection`. CRLFsuite supports `single URL`, `multiple URLs`, `cookies`, `GET,POST methods`.

## Installation

```
$ git clone https://github.com/Nefcore/CRLFsuite.git
$ cd CRLFsuite
$ sudo python3 setup.py install
$ crlfsuite -h
```
## Usage

Single URL scanning:

```
$ crlfsuite -u "http://testphp.vulnweb.com"
```

Multiple URLs scanning:

```
$ crlfsuite -i targets.txt
```

Specifying cookies:

```
$ crlfsuite -u "http://testphp.vulnweb.com" --cookies "key=val; newkey=newval"
```

Using POST method:

```
$ crlfsuite -i targets.txt -m POST -d "key=val&newkey=newval"
```

## License

<a href="https://github.com/Nefcore/CRLFsuite/blob/main/LICENSE">MIT LICENSE</a>
