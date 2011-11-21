= Unstubbing Base64 =

This exists because httpclientandroidlib uses android.util.Base64. When run
somewhere other than a device, this library is stubbed out. The alternatives --
code transformation to switch between org.apache.http and
ch.boye.httpclientandroidlib, and fixing a transformed version to use some old
version of commons-codec -- are even less pleasant.

Please forgive me.
