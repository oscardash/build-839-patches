Build #839 has git hash:

Revision: 7b074713782b1dd2f91bff371011fd7085cfdaf5

Obtain this revision and then apply the patches like this:

```
git am -3 -k < dashboard_enhancements.patch
```

and

```
git am -3 -k < cellphone.patch
```


These patches were generated with the following commands:

```
git format-patch -k --stdout fd45ee62d3790058413bbc3e446e386b4d440d3c..b105f177130d0b5d5a9d2a463da619e3b2dc6106 > cellphone.patch
```

```
git format-patch -k --stdout  4e16f2d7bdfdaa98429524dd2805a6bc952b6e6f..c38e47f012525fa5f98a9d2691513c30e254bc5b > dashboard_enhancements.patch
```

Note: Before an OSCAR user can view the dashboard of another OSCAR user, they require the security object "_dashboardChgUser".  The database update "database/mysql/updates/update-2018-11-11.sql" is provided to insert that "objectName" into "secObjectName".
