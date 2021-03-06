# py-tzone

**py-tzone** is a package to find the details for a timezone Like abbreviation or offset of any timezone from pytz import ```all_timezones```.

# Installation

This package can either be installed using pip or from a tarball using the standard Python distutils.

If you are installing using ```pip```, you don’t need to download anything as the latest version will be downloaded for you from PyPI:

```
pip install py-tzone
```
# Example & Usage

Import the method ```get_tz_details``` from ```py_tzone```

```python
from py_tzone import get_tz_details

tz_details = get_tz_details('Europe/Amsterdam')
print(tz_details)
```

```python
{
  'value': 'W. Europe Standard Time',
  'abbr': 'WEDT',
  'offset': 2, 
  'isdst': True,
  'text': '(UTC+01:00) Amsterdam, Berlin, Bern, Rome, Stockholm, Vienna',
  'utc':['Arctic/Longyearbyen', 'Europe/Amsterdam', 'Europe/Andorra', 'Europe/Berlin',
        'Europe/Busingen', 'Europe/Gibraltar', 'Europe/Luxembourg','Europe/Malta','Europe/Monaco', 
        'Europe/Oslo', 'Europe/Rome', 'Europe/San_Marino',                                               
        'Europe/Stockholm', 'Europe/Vaduz', 'Europe/Vatican', 'Europe/Vienna','Europe/Zurich']
 }
```


# What is UTC

`UTC` is Coordinated Universal Time. It is a successor to, but distinct from, Greenwich Mean Time (GMT) and the various definitions of Universal Time. UTC is now the worldwide standard for regulating clocks and time measurement.

All other timezones are defined relative to UTC, and include offsets like UTC+0800 - hours to add or subtract from UTC to derive the local time. No daylight saving time occurs in UTC, making it a useful timezone to perform date arithmetic without worrying about the confusion and ambiguities caused by daylight saving time transitions, your country changing its timezone, or mobile computers that roam through multiple timezones.

