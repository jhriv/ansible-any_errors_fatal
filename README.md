# Ansible Any Errors Fatal

To test the effect of `any_errors_fatal` directive, run the following
playbooks:

- `random_fail.yml` default values
- `random_fail-any_errors_fatal-false.yml` set to false, the default value
- `random_fail-any_errors_fatal-true.yml` set to true

Notice that in the first two playbooks, a host failing will allow the remaining
hosts to continue to the remaining tasks. In the final playbook, a failure of
any host will cause the playbook to stop on that play.
