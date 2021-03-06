Changelog
=========


v2.1.0 (2017-07-27)
-------------------
- Bump version to 2.1.0. [Robin Thomas]
- Safely perform _cellrepr on list objects, since list objects can be
  cell values (#7) [Robin Thomas]

  in a DataFrame. Deal with regression where float precision is mangled
  during round-trip testing, by using repr() on float values and str()
  on other values.

  Fixes #6.
- Complete basic write test. [Robin Thomas]
- Remove stray print stmt. [Robin Thomas]


v2.0.1 (2017-03-31)
-------------------
- CHANGELOG for 2.0.1. [Robin Thomas]
- Bump version to 2.0.1. [Robin Thomas]
- Fixing #4: Respecting the minimum number of cols (#5) [Thorbjørn Wolf]
- Overcome bad default repository url for upload_sphinx. [Robin Thomas]
- Switch to upload3 package. [Robin Thomas]


v2.0.0 (2017-03-29)
-------------------
- Changelog for v2.0.0. [Robin Thomas]
- Get_as_dataframe uses pandas TextParser (#3) [Robin Thomas]

  * pretty easy to hook up TextParser; let's see how all of the option
    handling works in later commits.

  * support evaluate_formulas

  * added basics of unit test suite, with accurate mock worksheet cell feed.

  * strip google sheet ID just to make mock XML smaller

  * fixed docs; added dev requirements in prep to use gitchangelog

  * gitchangelog.rc

  * gitchangelog config file in proper location

  * added latest generated CHANGELOG

  * externalized VERSION file; nearly complete test suite

  * completed test suite

  * updated CHANGELOG

  * back to 2.6-friendly %-based string formatting

  * dispensed with the now-silly-looking lazy ImportError for pandas import.

  * mention pandas.read_csv keyword argument support in README

  * avoid misinterpretation of ** in docstring by sphinx.

  * tighten up all the sphinx stuff

  * show |version| in docs index. parse version properly.

  * remove duplicate sphnix req

  * unworking attempt; need ws entry from worksheets feed to make
    a fully-functioning mock worksheet for writes.

  * write test works now

  * fix bytes/str problem in tests


v1.1.0 (2017-03-28)
-------------------
- LICENSE file via metadata, and correct upload-dir for docs. [Robin
  Thomas]
- Change default include_index=False since that's the common case. Bump
  version to 1.1.0. Complete documentation index.rst. [Robin Thomas]


v1.0.0 (2017-03-28)
-------------------
- List Pandas as dep. [Robin Thomas]
- Aded some sphinx support for steup cfg. [Robin Thomas]
- Initial pre-release commit. [Robin Thomas]
- Initial commit. [Robin Thomas]


