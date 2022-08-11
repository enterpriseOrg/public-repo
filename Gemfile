source 'https://rubygems.org'
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby '~> 2.7.1'
# frozen_string_literal: true

source 'https://rubygems.org'

# Authorization
gem 'declarative_policy', '~> 1.1.0'

# Authentication libraries
gem 'devise', '~> 4.7.2'
gem 'bcrypt', '~> 3.1', '>= 3.1.14'
gem 'doorkeeper', '~> 5.5.0.rc2'
gem 'doorkeeper-openid_connect', '~> 1.7.5'
gem 'rexml', '~> 3.2.5'
gem 'ruby-saml', '~> 1.13.0'
gem 'omniauth', '~> 1.8'
gem 'omniauth-auth0', '~> 2.0.0'
gem 'omniauth-azure-activedirectory-v2', '~> 1.0'
gem 'omniauth-azure-oauth2', '~> 0.0.9' # Deprecated v1 version
gem 'omniauth-cas3', '~> 1.1.4'
gem 'omniauth-dingtalk-oauth2', '~> 1.0'
gem 'omniauth-facebook', '~> 4.0.0'
gem 'omniauth-github', '~> 1.4'
gem 'omniauth-gitlab', '~> 1.0.2'
gem 'omniauth-google-oauth2', '~> 0.6.0'
gem 'omniauth-kerberos', '~> 0.3.0', group: :kerberos
gem 'omniauth-oauth2-generic', '~> 0.2.2'
gem 'omniauth-saml', '~> 1.10'
gem 'omniauth-shibboleth', '~> 1.3.0'
gem 'omniauth-twitter', '~> 1.4'
gem 'omniauth_crowd', '~> 2.4.0'
gem 'omniauth-authentiq', '~> 0.3.3'
gem 'gitlab-omniauth-openid-connect', '~> 0.8.0', require: 'omniauth_openid_connect'
gem 'omniauth-salesforce', '~> 1.0.5'
gem 'omniauth-atlassian-oauth2', '~> 0.2.0'
gem 'rack-oauth2', '~> 1.16.0'
gem 'jwt', '~> 2.1.0'

# Kerberos authentication. EE-only
gem 'gssapi', group: :kerberos

# Spam and anti-bot protection
gem 'recaptcha', '~> 4.11', require: 'recaptcha/rails'
gem 'akismet', '~> 3.0'
gem 'invisible_captcha', '~> 1.1.0'

# Two-factor authentication
gem 'devise-two-factor', '~> 4.0.0'
gem 'rqrcode-rails3', '~> 0.1.7'
gem 'attr_encrypted', '~> 3.1.0'
gem 'u2f', '~> 0.2.1'

# GitLab Pages
gem 'validates_hostname', '~> 1.0.11'
gem 'rubyzip', '~> 2.0.0', require: 'zip'
# GitLab Pages letsencrypt support
gem 'acme-client', '~> 2.0', '>= 2.0.6'

# Browser detection
gem 'browser', '~> 4.2'

# OS detection for usage ping
gem 'ohai', '~> 16.10'

# GPG
gem 'gpgme', '~> 2.0.19'

# LDAP Auth
# GitLab fork with several improvements to original library. For full list of changes
# see https://github.com/intridea/omniauth-ldap/compare/master...gitlabhq:master
gem 'gitlab_omniauth-ldap', '~> 2.1.1', require: 'omniauth-ldap'
gem 'net-ldap', '~> 0.16.3'

# API
gem 'grape', '~> 1.5.2'
gem 'grape-entity', '~> 0.10.0'
gem 'rack-cors', '~> 1.0.6', require: 'rack/cors'

gem 'rack-proxy', '~> 0.6.0'

gem 'sassc-rails', '~> 2.1.0'
gem 'autoprefixer-rails', '10.2.5.1'
gem 'terser', '1.0.2'

gem 'addressable', '~> 2.8'
gem 'tanuki_emoji', '~> 0.5'
gem 'gon', '~> 6.4.0'
gem 'request_store', '~> 1.5'
gem 'base32', '~> 0.3.0'

gem 'gitlab-license', '~> 2.0'

# Protect against bruteforcing
gem 'rack-attack', '~> 6.3.0'

# Sentry integration
gem 'sentry-raven', '~> 3.1'

# PostgreSQL query parsing
#
gem 'pg_query', '~> 2.1'

gem 'premailer-rails', '~> 1.10.3'

# LabKit: Tracing and Correlation
gem 'gitlab-labkit', '~> 0.21.1'
# Thrift is a dependency of gitlab-labkit, we want a version higher than 0.14.0
# because of https://gitlab.com/gitlab-org/gitlab/-/issues/321900
gem 'thrift', '>= 0.14.0'

# I18n
gem 'ruby_parser', '~> 3.15', require: false
gem 'rails-i18n', '~> 6.0'
gem 'gettext_i18n_rails', '~> 1.8.0'
gem 'gettext_i18n_rails_js', '~> 1.3'
gem 'gettext', '~> 3.3', require: false, group: :development

gem 'batch-loader', '~> 2.0.1'

# Perf bar
gem 'peek', '~> 1.1'

# Snowplow events tracking
gem 'snowplow-tracker', '~> 0.6.1'

# Metrics
gem 'method_source', '~> 1.0', require: false
gem 'webrick', '~> 1.6.1', require: false
gem 'prometheus-client-mmap', '~> 0.15.0', require: 'prometheus/client'

gem 'warning', '~> 1.2.0'

group :development do
  gem 'lefthook', '~> 0.7.0', require: false
  gem 'solargraph', '~> 0.43', require: false

  gem 'letter_opener_web', '~> 2.0.0'

  # Better errors handler
  gem 'better_errors', '~> 2.9.0'

  # thin instead webrick
  gem 'thin', '~> 1.8.0'

  gem 'sprite-factory', '~> 1.7'
end

group :development, :test do
  gem 'deprecation_toolkit', '~> 1.5.1', require: false
  gem 'bullet', '~> 6.1.3'
  gem 'pry-byebug'
  gem 'pry-rails', '~> 0.3.9'
  gem 'pry-shell', '~> 0.5.0'

  gem 'awesome_print', require: false

  gem 'database_cleaner', '~> 1.7.0'
  gem 'factory_bot_rails', '~> 6.2.0'
  gem 'rspec-rails', '~> 5.0.3'

  # Prevent occasions where minitest is not bundled in packaged versions of ruby (see #3826)
  gem 'minitest', '~> 5.11.0'

  gem 'png_quantizator', '~> 0.2.1', require: false

  gem 'parallel', '~> 1.19', require: false

  gem 'rblineprof', '~> 0.3.6', platform: :mri, require: false

  gem 'test_file_finder', '~> 0.1.3'
end

# Gems required in omnibus-gitlab pipeline
group :development, :test, :omnibus do
  # Using a fork until https://github.com/pivotal/LicenseFinder/pull/816 is
  # resolved. For details, check discussion in
  # https://gitlab.com/gitlab-org/gitlab/-/merge_requests/74881
  gem 'gitlab-license_finder', '~> 6.0', require: false
end

group :test do
  gem 'fuubar', '~> 2.2.0'
  gem 'rspec-retry', '~> 0.6.1'
  gem 'rspec_profiling', '~> 0.0.6'
  gem 'rspec-parameterized', require: false

  gem 'capybara', '~> 3.35.3'
  gem 'capybara-screenshot', '~> 1.0.22'
  gem 'selenium-webdriver', '~> 3.142'

  gem 'shoulda-matchers', '~> 4.0.1', require: false
  gem 'email_spec', '~> 2.2.0'
  gem 'webmock', '~> 3.9.1'
  gem 'rails-controller-testing'
  gem 'concurrent-ruby', '~> 1.1'
  gem 'test-prof', '~> 1.0.7'
  gem 'rspec_junit_formatter'
  gem 'guard-rspec'

  # Moved in `test` because https://gitlab.com/gitlab-org/gitlab/-/issues/217527
  gem 'derailed_benchmarks', require: false
end

gem 'octokit', '~> 4.15'

gem 'ya2yaml', '~> 0.31'

# https://gitlab.com/gitlab-org/gitlab/issues/207207
gem 'gitlab-mail_room', '~> 0.0.9', require: 'mail_room'

gem 'email_reply_trimmer', '~> 0.1'
gem 'html2text'

gem 'ruby-prof', '~> 1.3.0'
gem 'stackprof', '~> 0.2.15', require: false
gem 'rbtrace', '~> 0.4', require: false
gem 'memory_profiler', '~> 0.9', require: false
gem 'benchmark-memory', '~> 0.1', require: false
gem 'activerecord-explain-analyze', '~> 0.1', require: false

# OAuth
gem 'oauth2', '~> 1.4'

# Health check
gem 'health_check', '~> 3.0'

# System information
gem 'vmstat', '~> 2.3.0'
gem 'sys-filesystem', '~> 1.1.6'

# NTP client
gem 'net-ntp'

# SSH host key support
gem 'net-ssh', '~> 6.0'
gem 'sshkey', '~> 2.0'

# Required for ED25519 SSH host key support
group :ed25519 do
  gem 'ed25519', '~> 1.2'
  gem 'bcrypt_pbkdf', '~> 1.0'
end

# Spamcheck GRPC protocol definitions
gem 'spamcheck', '~> 0.1.0'

# Gitaly GRPC protocol definitions
gem 'gitaly', '~> 14.4.0.pre.rc43'

# KAS GRPC protocol definitions
gem 'kas-grpc', '~> 0.0.2'

gem 'grpc', '~> 1.30.2'

gem 'google-protobuf', '~> 3.17.1'

gem 'toml-rb', '~> 2.0'

# Feature toggles
gem 'flipper', '~> 0.21.0'
gem 'flipper-active_record', '~> 0.21.0'
gem 'flipper-active_support_cache_store', '~> 0.21.0'
gem 'unleash', '~> 3.2.2'
gem 'gitlab-experiment', '~> 0.6.5'

# Structured logging
gem 'lograge', '~> 0.5'
gem 'grape_logging', '~> 1.7'

# DNS Lookup
gem 'gitlab-net-dns', '~> 0.9.1'

# Countries list
gem 'countries', '~> 3.0'

gem 'retriable', '~> 3.1.2'

# LRU cache
gem 'lru_redux'

gem 'erubi', '~> 1.9.0'

# Locked as long as quoted-printable encoding issues are not resolved
# Monkey-patched in `config/initializers/mail_encoding_patch.rb`
# See https://gitlab.com/gitlab-org/gitlab/issues/197386
gem 'mail', '= 2.7.1'
gem 'mail-smtp_pool', '~> 0.1.0', path: 'vendor/gems/mail-smtp_pool', require: false

# File encryption
gem 'lockbox', '~> 0.6.2'

# Email validation
gem 'valid_email', '~> 0.1'

# JSON
gem 'json', '~> 2.5.1'
gem 'json_schemer', '~> 0.2.18'
gem 'oj', '~> 3.10.6'
gem 'multi_json', '~> 1.14.1'
gem 'yajl-ruby', '~> 1.4.1', require: 'yajl'

gem 'webauthn', '~> 2.3'

# IPAddress utilities
gem 'ipaddress', '~> 0.8.3'

gem 'parslet', '~> 1.8'

gem 'ipynbdiff', '0.3.8'
