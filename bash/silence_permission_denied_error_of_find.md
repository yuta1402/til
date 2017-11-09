# Silence permission denied error of find
findで`/`から検索をするとpermission deniedのエラーが出てくるのでみにくい。
```
find / -name "filename" 2> /dev/null
```
上記のようにfindの標準エラーを`/dev/null`に出力することで対応する。
