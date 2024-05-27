# SUIT-Report
Secure status reporting for SUIT manifests 

* [draft-ietf-suit-report](./draft-ietf-suit-report.md)

## Converting draft from md file

### Prerequisite packages

Requires two packages:
```
kramdown-rfc2629 by Ruby
xml2rfc by Python
```

Installing required packages on Fedora
```
sudo dnf makecache
sudo dnf -y install python3-pip git make gem
gem install kramdown-rfc2629
pip3 install xml2rfc
```

Installing required packages on Ubuntu
```
sudo apt-get update
sudo apt-get -y install python3-pip ruby git curl
pip3 install xml2rfc
gem install kramdown-rfc2629
```

### Generating draft from a markdown file

```
git clone https://github.com/suit-wg/suit-report.git
cd suit-report
make
```

It will create `draft-ietf-suit-report-latest.txt` and
`draft-ietf-suit-report-latest.xml`.

## Submitting draft

TBD
