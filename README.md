# Redmine Code Audit [![Build Status](https://travis-ci.org/eXolnet/redmine-code-audit.svg)](https://travis-ci.org/eXolnet/redmine-code-audit)

Code Audit is a Redmine plugin that allows users to post audits on commits in repositories linked to projects.

## Getting started

1. Follow the Redmine plugin installation steps at: http://www.redmine.org/wiki/redmine/Plugins and make sure the plugin is installed to `vendor/plugins/redmine_code_audit`
2. Restart your Redmine web servers (e.g. mongrel, thin, mod_rails)
3. Login and enable the "Audit" module on the projects you want to use it.

## Testing/sending out emails

The VM is configured to use Postfix to send outgoing emails. In order for it to work properly (in other words have the emails not rejected by the receiving server), make sure that the emission email adress in `Administration - Settings - Email notifications` is configured.

# Contributing

* `rake redmine:plugins:migrate RAILS_ENV=production`
