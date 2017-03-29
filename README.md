# Innovator Service Desk (ITIL)

The Innovator Service Desk Solution (ISD) is based on the OGC's concept of IT Service Management which is outlined in Infrastructure Technology Infrastructure Library (ITIL) Specification (v2).

In addition to the guidelines outlined by the OGC, the ISD Solution also includes capabilities outlined by the members of the IPT.

The primary focus of the Service Desk in an ITIL environment is to restore service as quickly as possible. The ISD Solution serves as the single point of contact between users and IT Service Management.

The ISD Solution includes functionality in the following key areas:

* Incident Management
* Problem Management
* Change Management
* Service Level Management
* Email Integration

## History

This project and the following release notes have been migrated from the old Aras Projects page. Unlike community projects that have been migrated and archived, this project will be updated for compatibility with the latest release of Aras Innovator.

Release | Notes
--------|--------
[v1](https://github.com/ArasLabs/innovator-service-desk/releases/tag/v1) | This is the initial Phase-I build for the community.

#### Supported Aras Versions

Project | Aras
--------|------
[v1](https://github.com/ArasLabs/innovator-service-desk/releases/tag/v1) | 8.2.0

## Installation

#### Important!
**Always back up your code tree and database before applying an import package or code tree patch!**

### Pre-requisites

1. Aras Innovator installed (version 11.0 SPx preferred)
2. Aras Package Import tool
3. **com.aras.innovator.solution.ITIL** import package
4. innovator-service-desk code tree overlay

### Install Steps

1. Backup your code tree and store the backup in a safe place.
2. Copy the Innovator folder from the project's CodeTree subdirectory.
3. Paste the Innovator folder into the root directory of your Aras installation.
  * Tip: This is the same directory that contains the InnovatorServerConfig.xml file.
4. Backup your database and store the BAK file in a safe place.
5. Open up the Aras Package Import tool.
6. Enter your login credentials and click **Login**
  * _Note: You must login as root for the package import to succeed!_
7. Enter the package name in the TargetRelease field.
  * Optional: Enter a description in the Description field.
8. Enter the path to your local `..\innovator-service-desk\Import\ITIL.mf` file in the Manifest File field.
9. Select **com.aras.innovator.solution.ITIL** in the Available for Import field.
10. Select Type = **Merge** and Mode = **Thorough Mode**.
11. Click **Import** in the top left corner.
12. Close the Aras Package Import tool.

## Usage

See [Innovator 8.2 ISD Solution Guide v1a](./Documentation/Innovator%208.2%20ISD%20Solution%20Guide%20v1a.pdf) for more information on using this project.

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

For more information on contributing to this project, another Aras Labs project, or any Aras Community project, shoot us an email at araslabs@aras.com.

## Credits

Created by Russ Moro for Aras Corporation.

## License

Aras Labs projects are published to Github under the MIT license. See the [LICENSE file](./LICENSE.md) for license rights and limitations.
