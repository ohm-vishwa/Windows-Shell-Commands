# Windows Shell Commands
## Diskpart 
> Open treminal and then, type
```bash
diskpart
```

> check no. of disks
```bash
list disk
```

> Select Primary disk
```
sel disk 0
```

> see partitions
```bash
list partition
```

> to delete a partiton
```bash
sel partition <partition_number>
delete partition 
```

> if not deleted then,
```bash
delete partition override
```

> see volumes
```bash
list vol
```

> to delete a particular volume
```
list vol
sel vol <vol_number/letter>
delete vol
```
> if not deleted then use,
```bash
delete vol override
```

> to hide particular volume
```bash
list vol
remove letter = <vol_letter>
```

> to unhide particular volume
```bash
list vol
sel vol <vol_number>
assign letter = <any_letter>
```

## format SD Card
> you need to insert then,
```bash 
diskpart
```

```bash
list disk
```

```bash
sel disk <disk_no_of_sd_card>
```

> format ` ntfs `
```bash
format fs=ntfs quick
```

> format ` fat32 `
```bash
format fs=fat32 quick
```