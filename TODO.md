# TODO

* Add an optional YAML file for project settings, such as ignoring certain rules for certain resources
* Region is hard-coded to us-east-1 for GetValueFromS3
* Use type switch as more idiomatic way to handle multiple types in match.go
* Use log package for error reporting
* Deal with a few FIXME comments in code, mostly error handling
* Would it be useful to have helper utilities to send output to CloudWatch/SNS/Kinesis?
* Update value_from to handle JSON return values
* Create a Provider interface for AWS calls, create a mock for testing SecurityGroupLinter
* Starting to have inconsistent naming in ops: is-true, is-false, has-properties vs. present, absent, empty, null
* Add options to Assertion type, for things like 'ignore-case' for string compares? Or just use a regex?
* Provide a default -query of 'Violations[]', and add an option for a full report
* Document conditions
* For Terraform, variables are currently parsed per file, but should be across all files provided