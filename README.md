# qualys-export

[![Build Status](https://api.travis-ci.org/nortonlifelock/qualys-export.svg?branch=master)](https://travis-ci.org/nortonlifelock/qualys-export)
[![Go Report Card](https://goreportcard.com/badge/github.com/nortonlifelock/qualys-export)](https://goreportcard.com/report/github.com/nortonlifelock/qualys-export)
[![GoDoc](https://godoc.org/github.com/nortonlifelock/qualys-export?status.svg)](https://godoc.org/github.com/nortonlifelock/qualys-export)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

qualys-export


Command: qualys-export

Example Call: ```qualys-export -config app.json -cpath "path to config" -org ORGCODE```

The tool will prompt for the asset group(s) that should be exported as seen below

Enter Asset Groups to Export (Comma Separated): 55555,77777

NOTE: This tool takes some time because of it's dependency on the download of the Knowledge Base from Qualys. 

NOTE: This tool may also contain duplicate rows because of how the Qualys API orders the records

Output Format
QID	| IP | HOSTNAME | OS | VULNERABILITY | ACTIVEKERNEL	| PORTS	| CVSS | CVE | LASTDETECTED

