# Desktop Metres

Custom [Rainmeter](https://www.rainmeter.net/) skin inspired by [this post](https://www.hwinfo.com/forum/threads/my-rainmeter-skin.3489/).

![Sample of skin](Sample.png)

## HWiNFO setup

The skin reads HWiNFO's shared registry values from:

`HKEY_CURRENT_USER\SOFTWARE\HWiNFO64\VSB`

The existing sensor order is defined by the `*Index` variables near the top of `desktop_meters.ini`.

Network speed is scaled to my max network speed (750Mbps) but can be changed to match yours

The GPU memory sensor I selected supplies a percentage rather than a byte count. `VramTotalBytes` is therefore set to `17179869184` (16 GiB) for the current GPU. Change that variable if the skin is used with a different graphics card.

Number of CPU threads is not dynamic so would need to be manually changed if you've more or less

Also, doesn't dynamically detect additional drives. Would need additional HwInfo values adding
