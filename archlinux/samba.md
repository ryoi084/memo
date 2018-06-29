# Sambaのダウンロードとwindowsとの共有方法

[Sambaを使いUbuntuとWindowsとの間でファイル共有する](https://qiita.com/KentaKawamata/items/8bee9e02e74565b6c147)

実際に実行をしたときは,

```
    systemctl enable smb nmb
```
で実行を行った.

また設定ファイルである```/etc/samba/smb.conf```はarch wikiに記述されているように

``` wget "https://git.samba.org/samba.git/?p=samba.git;a=blob_plain;f=examples/smb.conf.default;hb=HEAD" -O /etc/samba/smb.conf ```

で持ってくることで解決した.

また最後尾に

```
    [share]
```
という名前で設定を行い実行した.