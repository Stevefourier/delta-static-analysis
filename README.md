#Delta Static Analysis Tool for npm Packages to Detect Malicious Updates

## Overview

This is a command-line tool designed for detecting malicious code in npm packages. It provides functionality to scan packages, run evaluations, and obtain overall update frequency information.
For its detection it relies on the static code analysis tool CodeQL. 

A query set for the detection of suspicious behavior in JavaScript code is provided in the directory xy. 
The tool will compare the CodeQL results resp. findings of two versions to identify the new findings of the second version, relevant for the detection. 
The severity values of these differential findings will sumed up and compared to a predfined threshold, determining whether a certain update is flagged as potentially malicious.
