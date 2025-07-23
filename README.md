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
pip3 install xml2rfc
gem install kramdown-rfc2629 cddl cddlc
```

Installing required packages on Ubuntu
```
sudo apt-get update
sudo apt-get -y install python3-pip ruby git curl
pip3 install xml2rfc
gem install kramdown-rfc2629 cddl cddlc
```

### Generating draft from a markdown file

```
git clone https://github.com/suit-wg/suit-report.git
cd suit-report
make
```

It will create `draft-ietf-suit-report.txt`, `draft-ietf-suit-report.xml` and `draft-ietf-suit-report.html`

## Conduct CDDL syntax check

To check the cddl syntax whenever making changes in the cddl file

```
make -C cddl
```

## Updating repo on GitHub

Make updates to the `draft-ietf-suit-report.md` and/or `draft-ietf-suit-report.cddl`.
Regenerate xml, txt and html with `make` command.

Commit and push to GitHub the changes on all files listed below.
```
draft-ietf-suit-report.md
draft-ietf-suit-report.cddl
```

## Submitting draft

TBD
