# d88split

Splits concatenated D88/D77 disk images.
* **D88** is an image format for NEC PC-88/PC-98 floppy disks.
* **D77** is the same format for Fujitsu FM77 series computers.
Written in Perl, released to the public domain.

## Examples

List images packed in a file:
```
% ./d88split.pl l kohaku.d77
 Image                           Bytes 
---------------------------------------
Kohaku_1                        473776
Kohaku_2                        473776
Kohaku_3                        473776
Kohaku_4                        473776
```

Extract images:
```
% ./d88split.pl e kohaku.d77
Kohaku_1 => kohaku#1.d77 ( 473776 bytes)
Kohaku_2 => kohaku#2.d77 ( 473776 bytes)
Kohaku_3 => kohaku#3.d77 ( 473776 bytes)
Kohaku_4 => kohaku#4.d77 ( 473776 bytes)
```
