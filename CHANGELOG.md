## 0.14.0 (August 19, 2021)

ENHANCEMENTS:

* Add map output for client and secret ids (thanks @dmytro-dorofeiev)

## 0.13.0 (August 10, 2021)

ENHANCEMENTS:

* Add support for Cognito Identity Providers (thanks @bobdoah)

## 0.12.0 (July 4, 2021)

FIXES:

* set client_secrets output to be sensitive (thanks @sapei)

## 0.11.1 (May 21, 2021)

FIXES:

* Revert prevent_destroy due to [Variables may not be used here issue](https://github.com/hashicorp/terraform/issues/22544)

## 0.11.0 (May 21, 2021)

ENHANCEMENTS:

* Add support to prevent the user pool from being destroyed (thanks @Waschnick)

## 0.10.5 (May 12, 2021)

FIXES:

* Fix incorrect example with `access_token_validity` (thanks @tsimbalar)

## 0.10.4 (April 25, 2021)

FIXES:

* Add `depends_on` servers in `aws_cognito_user_pool_client.client` resource

## 0.10.3 (April 15, 2021)

FIXES:

* Make code formatting works with Terraform >= 0.14 (Thanks @stevie-)

## 0.10.2 (April 10, 2021)

FIXES:

* Remove lifecycle for schema addition ([issue](https://github.com/hashicorp/terraform-provider-aws/pull/18512) fixed in the AWS provider)

## 0.10.1 (April 10, 2021)

FIXES:

* Update complete example

## 0.10.0 (April 10, 2021)

ENHANCEMENTS:

* Add support for `access_token_validity`, `id_token_validity` and `token_validity_units`
* Update complete example with `access_token_validity`, `id_token_validity` and `token_validity_units`

## 0.9.4 (February 14, 2021)

FIXES:

* Update README to include schema changes know issue

## 0.9.3 (January 27, 2021)

ENHANCEMENTS:

* Update description for `enabled` variable


## 0.9.2 (January 27, 2021)

ENHANCEMENTS:

* Update conditional creation example

## 0.9.1 (January 27, 2021)

FIXES:

* Set default value for enable variable to `true`

## 0.9.0 (January 24, 2021)

ENHANCEMENTS:

* Support conditional creation (thanks @Necromancerx)

## 0.8.0 (December 28, 2020)

ENHANCEMENTS:

* Add support for support `account_recovery_setting`

## 0.7.1 (December 11, 2020)

FIXES:

* Ignore schema changes and prevent pool destruction

## 0.7.0 (November 25, 2020)

ENHANCEMENTS:

* Add `from_email_address`

## 0.6.2 (August 13, 2020)

FIXES:

* Update CHANGELOG

## 0.6.1 (August 13, 2020)

ENHANCEMENTS:

* Change source in examples to use Terraform format

FIXES:

* Add `username_configuration` dynamic block to avoid forcing a new resource when importing a user pool
* Remove `case_sensitive` variable. Use the `username_configuration` map variable to define the `case_sensitive` attribute

UPDATES:

* Updated README and examples

## 0.5.0 (July 31, 2020)

FIXES:

* Depcreate support to `unused_account_validity_days`
* Update README and examples removing any reference to the deprecated `unused_account_validity_days` field

## 0.4.0 (May 2, 2020)

ENHANCEMENTS:

* Add support for `software_token_mfa_configuration`

## 0.3.3 (April 24, 2020)

FIXES:

* Applies `case_sensitive` via `username_configuration`

## 0.3.2 (April 24, 2020)

UPDATE:

* Update README with `case_sensitive`

## 0.3.1 (April 24, 2020)

ENHANCEMENTS:

* Add `case_sensitive` for `aws_cognito_user_pool`

## 0.3.0 (April 1, 2020)

ENHANCEMENTS:

* Add `param client_prevent_user_existence_errors` for client

UPDATES:

* Add Terraform logo in README

## 0.2.2 (March 16, 2020)

FIXES:

* Fix typo in comments

## 0.2.1 (February 6, 2020)

BUG FIXES:

* Cognito unused_account_validity_days bug with 2.47:  The aws-provider reports the existence of the `unused_account_validity_days` even if it was never declared, automatically matching the new `temporary_password_validity_day`

## 0.2.0 (February 5, 2020)

UPDATES:

* AWS Provider 2.47.0: Deprecate unused_account_validity_days argument and add support for temporary_password_validity_days argument

## 0.1.0 (November 23, 2019)

FEATURES:

  * Module implementation
