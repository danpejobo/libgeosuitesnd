# Parser for the GeoSuite[tm] SND export format

This library provides functionality to parse geotechnical investigation data in `.snd` files generated by GeoSuite.

Usage:

```
>>> libgeosuitesnd.parse("SOMEFILE.SND" )
[{'method_code': 23,
  'method_name': 'rps',
  'day': 23,
  'month': 5,
  'year': 2011,
  'date': '2011-5-23',
  'stop_code': 91,
  'stop_desc': 'abandoned_hit_hard_surface',
  'data':        depth  feed_force  flushing  extra_spin  hammering  pumping comments
  0      0.021       102.0         0           0          0        0         
  1      0.042      1318.0         0           0          0        0         
  2      0.052      1038.0         0           0          0        0         
  3      0.072      1101.0         0           0          0        0         
  4      0.100      1728.0         0           0          0        0         
  ...      ...         ...       ...         ...        ...      ...      ...
  1326  28.550      5301.0         0           1          0        0         
  1327  28.570      9423.0         0           1          0        0         
  1328  28.605     12217.0         0           1          0        0         
  1329  28.631     11564.0         0           1          0        0         
  1330  28.650     11942.0         0           1          0        0         
  
  [1331 rows x 7 columns],
  'depth_increment': 0.021,
  'depth_bedrock': None,
  'x': 288557.381,
  'y': 6667259.708,
  'z': 139.01}]
```
