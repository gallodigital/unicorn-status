# unicorn_status.rb - modified to send metrics to CloudWatch

Sends information to CloudWatch every few seconds (specified on command line) about what's in a given Unicorn socket.
It also logs the information to STDOUT, if you're into that kind of thing.

Usage:

    ruby unicorn_status.rb /path/to/your/unicorn/socket.sock 10

Setup:

    gem install unicorn aws-sdk

Bugs/Contributions:
Pull requests welcome. Enhancements, bugfixes, whatever, it's all good. Fork, do work, test and submit a pull request.

Contributors:
 - Chris Rigor (https://github.com/crigor)
 - Adam Holt (https://github.com/omgitsads)
 - J. Austin Hughey (https://github.com/jaustinhughey)
 - Keith Gable (https://github.com/ziggythehamster)

License: CC Attribution 3.0 Unported (http://creativecommons.org/licenses/by/3.0/)

## AWS notes

This script expects that you are using IAM instance roles, and that the instance role has permission to put metrics.
