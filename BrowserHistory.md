# Browser History
# Chrome
* https://www.foxtonforensics.com/browser-history-examiner/chrome-history-location
## Location of Google Chrome history
### Windows Vista, 7, 8, 10
```
C:\Users\<username>\AppData\Local\Google\Chrome\User Data\Default
C:\Users\<username>\AppData\Local\Google\Chrome\User Data\Default\Cache
```
### Windows XP
```
C:\Documents and Settings\<username>\Local Settings\Application Data\Google\Chrome\User Data\Default
C:\Documents and Settings\<username>\Local Settings\Application Data\Google\Chrome\User Data\Default\Cache
```
### Mac OS X
```
/Users/<username>/Library/Application Support/Google/Chrome/Default
/Users/<username>/Library/Caches/Google/Chrome/Default/Cache
```
### Linux/Unix
```
/home/<username>/.config/google-chrome/Default
/home/<username>/.cache/google-chrome/Default/Cache
```
## Format of Google Chrome history
### Bookmarks
Chrome Bookmarks are stored in the 'Bookmarks' JSON file.
### Cache
Chrome Cache is stored using an Index file ('index'), a number of Data Block files ('data_#'), and a number of separate data files ('f_######').
### Cookies
Chrome Cookies are stored in the 'Cookies' SQLite database, within the 'cookies' table.
### Downloads
Chrome Downloads are stored in the 'History' SQLite database, within the 'downloads' and 'downloads_url_chains' tables.
### Favicons
Chrome Favicons are stored in the 'Favicons' SQLite database, within the 'favicons', 'favicon_bitmaps' and 'icon_mapping' tables. Older versions of Chrome stored Favicons in a 'Thumbnails' SQLite database, within the 'favicons' table.
### Form History
Chrome Form History is stored in the 'Web Data' SQLite database, within the 'autofill' table. Older versions of Chrome stored associated dates within an 'autofill_dates' table.
### Logins
Chrome Logins are stored in the 'Login Data' SQLite database, within the 'logins' table. Older versions of Chrome stored Logins in the 'Web Data' SQLite database.
### Searches
Chrome Searches are stored in the 'History' SQLite database, within the 'keyword_search_terms' table. Associated URL information is stored within the 'urls' table.
### Session Data
Chrome Session Data is stored in the 'Current Session', 'Current Tabs', 'Last Session' and 'Last Tabs' files.
### Thumbnails
Chrome Thumbnails are stored in the 'Top Sites' SQLite database, within the 'thumbnails' table. Older versions of Chrome stored Thumbnails in a 'Thumbnails' SQLite database, within the 'thumbnails' table.
### Website Visits
Chrome Website Visits are stored in the 'History' SQLite database, within the 'visits' table. Associated URL information is stored within the 'urls' table. Older versions of Chrome stored archived Website Visits in a separate 'Archived History' SQLite database, within the 'visits' table.

# Firefox
* https://www.foxtonforensics.com/browser-history-examiner/firefox-history-location
## Location of Mozilla Firefox history
### Windows Vista, 7, 8, 10
```
C:\Users\<username>\AppData\Roaming\Mozilla\Firefox\Profiles\<profile folder>
C:\Users\<username>\AppData\Local\Mozilla\Firefox\Profiles\<profile folder>\cache2
```
### Windows XP
```
C:\Documents and Settings\<username>\Application Data\Mozilla\Firefox\Profiles\<profile folder>
C:\Documents and Settings\<username>\Local Settings\Application Data\Mozilla\Firefox\Profiles\<profile folder>\cache2
```
### Mac OS X
```
/Users/<username>/Library/Application Support/Firefox/Profiles/<profile folder>
/Users/<username>/Library/Caches/Firefox/Profiles/<profile folder>/cache2
```
### Linux/Unix
```
/home/<username>/.mozilla/firefox/<profile folder>
/home/<username>/.cache/mozilla/firefox/<profile folder>/cache2
```
Up to version 31 the cache files were stored in a folder named 'Cache'. Starting with version 32 the cache files are stored in a folder named 'cache2'.

## Format of Mozilla Firefox history
### Bookmarks
Firefox Bookmarks are stored in the 'places.sqlite' database, within the 'moz_bookmarks' table. Associated URL information is stored within the 'moz_places' table.
### Cache
Firefox Cache is stored using a Cache Map File ('_CACHE_MAP_'), three Cache Block files ('_CACHE_00#_'), and a number of separate data files. The cache structure was changed in Firefox version 32 and named 'Cache v2'.
### Cookies
Firefox Cookies are stored in the 'cookies.sqlite' database, within the 'moz_cookies' table.
### Downloads
Firefox Downloads are stored in the 'places.sqlite' database, within the 'moz_annos' table. Associated URL information is stored within the 'moz_places' table. Older versions of Firefox stored Downloads in a separate 'downloads.sqlite' database, within the 'moz_downloads' table.
### Favicons
Firefox Favicons are stored in the 'favicons.sqlite' database, within the 'moz_icons' table. Older versions of Firefox stored Favicons in the 'places.sqlite' database, within the 'moz_favicons' table.
### Form History
Firefox Form History is stored in the 'formhistory.sqlite' database, within the 'moz_formhistory' table.
### Logins
Firefox Logins are stored in the 'logins.json' file. Older versions of Firefox stored Logins in a 'signons.sqlite' database, within the 'moz_logins' table.
### Searches
Firefox doesn't explicitly store Searches however they can be extracted from URLs within Website Visits, Session Data, Cache Records and Favicons.
### Session Data
Firefox Session Data is stored in JSON format within the 'sessionstore.jsonlz4' file.
### Thumbnails
Firefox Thumbnails are stored as individual PNG files within the 'thumbnails' folder.
### Website Visits
Firefox Website Visits are stored in the 'places.sqlite' database, within the 'moz_historyvisits' table. Associated URL information is stored within the 'moz_places' table.

# Microsoft Edge
* https://www.foxtonforensics.com/browser-history-examiner/microsoft-edge-history-location
On January 15th, 2020 Microsoft released Edge v79, the first stable version of their Chromium-based Edge web browser.

## Location of Microsoft Edge history (v79+)
### Windows 7, 8, 10
```
C:\Users\<username>\AppData\Local\Microsoft\Edge\User Data\Default
C:\Users\<username>\AppData\Local\Microsoft\Edge\User Data\Default\Cache
```
## Format of Microsoft Edge history (v79+)
### Bookmarks
Edge Bookmarks are stored in the 'Bookmarks' JSON file.
### Cache
Edge Cache is stored using an Index file ('index'), a number of Data Block files ('data_#'), and a number of separate data files ('f_######').
### Cookies
Edge Cookies are stored in the 'Cookies' SQLite database, within the 'cookies' table.
### Downloads
Edge Downloads are stored in the 'History' SQLite database, within the 'downloads' and 'downloads_url_chains' tables.
### Favicons
Edge Favicons are stored in the 'Favicons' SQLite database, within the 'favicons', 'favicon_bitmaps' and 'icon_mapping' tables.
### Logins
Edge Logins are stored in the 'Login Data' SQLite database, within the 'logins' table.
### Searches
Edge Searches are stored in the 'History' SQLite database, within the 'keyword_search_terms' table. Associated URL information is stored within the 'urls' table.
### Session Data
Edge Session Data is stored in the 'Current Session', 'Current Tabs', 'Last Session' and 'Last Tabs' files.
### Thumbnails
Edge Thumbnails are stored in the 'Top Sites' SQLite database, within the 'thumbnails' table.
### Website Visits
Edge Website Visits are stored in the 'History' SQLite database, within the 'visits' table. Associated URL information is stored within the 'urls' table.

## Location of Microsoft Edge history (up to v44)
### Windows 10
```
C:\Users\<username>\AppData\Local\Packages\<package name>\AC\MicrosoftEdge\User\Default\Favorites
C:\Users\<username>\AppData\Local\Packages\<package name>\AC\MicrosoftEdge\User\Default\Recovery
C:\Users\<username>\AppData\Local\Packages\<package name>\AC\MicrosoftEdge\User\Default\DataStore
C:\Users\<username>\AppData\Local\Microsoft\Windows\WebCache
```
## Format of Microsoft Edge history (up to v44)
### Bookmarks
Edge Bookmarks are stored in the 'spartan.edb' ESE database, within the 'Favorites' container. Older versions of Edge stored Bookmarks as separate Internet Shortcut (.url) files in the 'Favorites' folder.
### Cache
Edge Cache records are stored in the 'WebCacheV01.dat' ESE database, within the 'Content' containers. The cached files are stored as separate files in locations specified within the ESE database.
### Cookies
Edge Cookies are stored in the 'WebCacheV01.dat' ESE database, within the 'CookieEntryEx' containers. Older versions of Edge stored cookies as separate text files in locations specified within the ESE database.
### Downloads
Edge Downloads are stored in the 'WebCacheV01.dat' ESE database, within the 'iedownload' containers.
### Session Data
Edge Session Data is stored in a number of .dat files in the 'Recovery' folder.
### Website Visits
Edge Website Visits are stored in the 'WebCacheV01.dat' ESE database, within the 'History' containers.

# Internet Explorer
* https://www.foxtonforensics.com/browser-history-examiner/internet-explorer-history-location
## Location of Internet Explorer history
### Windows 7, 8, 10
```
C:\Users\<username>\Favorites
C:\Users\<username>\AppData\Local\Microsoft\Windows\WebCache
C:\Users\<username>\AppData\Local\Microsoft\Internet Explorer\Recovery
```

## Format of Internet Explorer history
### Bookmarks
Internet Explorer Bookmarks are stored in separate Internet Shortcut (.url) files within the 'Favorites' folder.
### Cache
Internet Explorer Cache records are stored in the 'WebCacheV01.dat' ESE database, within the 'Content' containers. The cached files are stored as separate files in locations specified within the ESE database.
### Cookies
Internet Explorer Cookie records are stored in the 'WebCacheV01.dat' ESE database, within the 'Cookies' containers. The cookie files are stored as separate files in locations specified within the ESE database.
### Downloads
Internet Explorer Downloads are stored in the 'WebCacheV01.dat' ESE database, within the 'iedownload' containers.
### Session Data
Internet Explorer Session Data is stored in a number of .dat files within the 'Recovery' folder.
### Website Visits
Internet Explorer Website Visits are stored in the 'WebCacheV01.dat' ESE database, within the 'History' containers.

