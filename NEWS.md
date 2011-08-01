What's New
----------

 * The put command now discards the entire job body before returning
   JOB_TOO_BIG. Previously, it interpreted the job body as commands. This was a
   potential security hole, where malicious users could craft job payload data
   to inject commands without cooperation from the beanstalk client
   application.
 * Fix issue #40 by requiring an absolute path when `-b` is used with `-d`.

Full list of changes in this release (includes authorship information):
<http://github.com/kr/beanstalkd/compare/v1.4.5...v1.4.6>

