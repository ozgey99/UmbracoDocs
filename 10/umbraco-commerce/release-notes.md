# Release Notes

In this section, we have summarized the changes to Umbraco Commerce in this particular major version and all of it's major/minor releases. For details of changes in other major versions, see the release notes of that specific versions documentation.

If there are any breaking changes or other issues to be aware of when upgrading they are also noted here.

{% hint style="info" %}
If you are upgrading to a new major version, check the breaking changes in the [Version Specific Upgrade Notes](getting-started/installation/version-specific-upgrades.md) article.
{% endhint %}

For details of releases for **Vendr**, refer to the [Change log file on Github](changelog-archive/Vendr-core.md).

## Release History

#### [10.0.5](https://github.com/umbraco/Umbraco.Commerce.Issues/issues?q=is%3Aissue+is%3Aclosed+label%3Arelease%2F10.0.5) (December 13th 2023)

* Fixed Cross-site scripting (XSS) issue in email/print templates.
  
#### [10.0.4](https://github.com/umbraco/Umbraco.Commerce.Issues/issues?q=is%3Aissue+is%3Aclosed+label%3Arelease%2F10.0.4) (November 1st 2023)

* Use Microsoft.Data.SqlClient for migrations to support Azure connection strings [#443](https://github.com/umbraco/Umbraco.Commerce.Issues/issues/443).
* Move system config files to `system.{}.config.json` to allow overriding as per the docs [#448](https://github.com/umbraco/Umbraco.Commerce.Issues/issues/448).
* Updated order/cart editor config to allow `template` option for custom property rendering [#446](https://github.com/umbraco/Umbraco.Commerce.Issues/discussions/446).

#### [10.0.3](https://github.com/umbraco/Umbraco.Commerce.Issues/issues?q=is%3Aissue+is%3Aclosed+label%3Arelease%2F10.0.3) (October 18th 2023)

* Fixed UI spelling mistakes as documented in issue [#427](https://github.com/umbraco/Umbraco.Commerce.Issues/issues/427).
* Fixed issue where adding a product with a uniqueness property, and then adding the same product without a uniqueness property would replace the initial orderline, rather than adding a new one [#438](https://github.com/umbraco/Umbraco.Commerce.Issues/issues/438)
* Fixed localization issue where `-1` in querystrings would get incorrectly formatted. Root ids are now formatted with an invarient culture.

#### [10.0.2](https://github.com/umbraco/Umbraco.Commerce.Issues/issues?q=is%3Aissue+is%3Aclosed+label%3Arelease%2F10.0.2) (September 13th 2023)

* Allow overriding of `SameSite`/`Path` for Umbraco Commerce cookies.
* Updated `productSource` resolution to check for both `IPublishedContent` and `IEnumerable<IPublishedContent>` as it depends on the picker used and what its return type is.

#### [10.0.1](https://github.com/umbraco/Umbraco.Commerce.Issues?q=is%3Aissue+is%3Aclosed+label%3Arelease%2F10.0.1) (August 15th 2023)

* Updated default order number template from `CART-{0}` to `ORDER-{0}`.
* Updated product adapter to resolve product details correctly from child node variants.

#### [10.0.0](https://github.com/umbraco/Umbraco.Commerce.Issues/issues?q=is%3Aissue+is%3Aclosed+label%3Arelease%2F10.0.0) (July 5th 2023)

* [Initial product launch](https://umbraco.com/blog/umbraco-commerce-release/).
