## Synopsis

Script to generate an html report from JTL files from JMeter using Perl

## Code Example

To modify the request you want to generate report for please fork the code and modify line 63 variable `@callNames`

## Motivation

Reduce the amount of time needed to generate a complete report from a JTL file generated using JMeter, instead of using Java and XSL transformation to generate reports, we generate aggregations using perl.
When the size of a JTL file is bigger than 2 GB XSL transformations are going to last more than 2 hours, with this script you can get a complete report in minutes.
This application was generated in order to let JMeter only generate an XML file for output, not doing any other operation to generate as much as request as we can.

## Installation

Only need [Perl][perl5] installed on your machine to run scripts.

[perl5]: http://www.perl.org/get.html

## Running

To generate a complete html summary with numbers of request, success, max, min average size and response times, percentiles, etc, same name as jtl file terminated by html.
	$ ./jtl2html <JTL_FILE>

## Example

Here you can find an example report.

## Contributing workflow

Here’s how we suggest you go about proposing a change to this project:

1. [Fork this project][fork] to your account.
2. [Create a branch][branch] for the change you intend to make.
3. Make your changes to your fork.
4. [Send a pull request][pr] from your fork’s branch to our `master` branch.

Using the web-based interface to make changes is fine too, and will help you
by automatically forking the project and prompting to send a pull request too.

[fork]: http://help.github.com/forking/
[branch]: https://help.github.com/articles/creating-and-deleting-branches-within-your-repository
[pr]: http://help.github.com/pull-requests/

## License

[MIT](./LICENSE).
