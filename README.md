# Simulator for UC integration drivers

This project is a simulator tool that reproduces the websocket requests between the UC Remote and the integration drivers : it acts like a remote and lets
- Launch and simulate the setup flow and fill in the input fields to configure the device(s) exposed by an integration driver
- Extract for each configured devices its entities, including : media players, sensors, selects (dropdown entities)
- Updates entities in realtime : media player (title, artwork, position...), sensor and select values
- Sends any media player command
- Handles media browsing and search media

Just run your integration driver (can be locally on your computer)
Set the following environment variables before running:  these must point to the IP and PORT of the running integration driver
Example :
```
export UC_INTEGRATION_INTERFACE=192.168.1.60
export UC_INTEGRATION_HTTP_PORT=9090
```
Just run `python test_driver.py`

You may need to run `python -m pip install -r requirements.txt` first


## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the
[tags and releases in this repository](https://github.com/albaintor/integration-kodi/releases).

## Changelog

The major changes found in each new release are listed in the [changelog](CHANGELOG.md)
and under the GitHub [releases](https://github.com/albaintor/integration-kodi/releases).

## Contributions

Please read our [contribution guidelines](CONTRIBUTING.md) before opening a pull request.

## License

This project is licensed under the [**Mozilla Public License 2.0**](https://choosealicense.com/licenses/mpl-2.0/).
See the [LICENSE](LICENSE) file for details.


