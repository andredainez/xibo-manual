<!--toc=getting_started-->

# [[PRODUCTNAME]] 1.8.8 - Codename "Tempel"

This is the eighth minor release of Xibo 1.8 Series. Included in this release are 34 bug fixes. There is a new Player with this release.

You can download this release from [GitHub - xibo-docker.tar.gz](https://github.com/xibosignage/xibo-cms/releases/download/1.8.8/xibo-docker.tar.gz). The full release files can be viewed [here](https://github.com/xibosignage/xibo-cms/releases/tag/1.8.8).

This release is a bug fix release for the 1.8 stable series. If you are upgrading from 1.4, 1.6 or 1.7 please refer to the [1.8.0 release notes](release_notes_1.8.0.html) for a detailed list of changes and upgrade notes.




## Requirements

[[PRODUCTNAME]] runs on [Docker](install_docker.html), please check the [install guide](install_cms.html) for detailed requirements. The archive for this release can be downloaded from [GitHub](https://github.com/xibosignage/xibo-docker/releases/tag/1.8.8).

The CMS can be run without Docker, but this is not our recommended configuration. Installs without Docker are called [Custom/Manual Installs](manual_install.html) and further details can be found [here](manual_install.html). The release archive for a manual install can be downloaded from [GitHub](https://github.com/xibosignage/xibo-cms/releases/tag/1.8.8).

We recommend using the 1.8.8 Windows Player with this release. The 1.7.6 or later version of the Windows Player is also compatible with this CMS, but will not run the latest features.



### Special Considerations

#### Changes to Modules

There are some important changes to modules in this release.

- `$this->concurrentRequestLock();` has been made `private` and can no longer be used from your own module code.
- `$this->concurrentRequestRelease();` has been made `private` and can no longer be used from your own module code.
- Widget HTML caching has been introduced so that by default HTML produced by Widgets is cached on a `widgetId` basis for 15 minutes and modified only when an option on the Widget is modified.
- Widget HTML caching can be adjusted in the Module code by implementing the caching methods, described in the [Modules Documentation](advanced_modules.html#rendering).




#### Switching to Docker

Our recommended configuration for 1.8 series onward will be based on Docker and from 1.8 the focus of the documentation has changed to reflect this. If you would like to try 1.8.8 by upgrading your existing 1.7 installation, we recommend switching to Docker. Please refer to the [upgrade guide for more information](upgrade_switch_to_docker.html).




## Upgrading

This release supports upgrades from 1.7.0 onwards. If you are running a release prior to 1.7.0 then please upgrade to [1.7.9](release_notes_1.7.9.html) first.

Follow the [upgrade](upgrade.html) instructions to complete the upgrade.



## Help

Please report problems with this release using the [Support Category on the Community Forum](https://community.xibo.org.uk/c/support).



## Issues addressed in this release

For a full list of enhancements and bug fixes please refer to the [Release Project Page](https://github.com/xibosignage/xibo/issues?q=milestone%3A1.8.8+is%3Aclosed).
