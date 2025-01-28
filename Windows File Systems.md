 # FAT File System
* FAT Stands for File Allocation Table. A few versions of FAT are FAT12, FAT16, FAT32 and exFAT.
## Deletion in FAT File System
* When a file is deleted in FAT, the first character of its directory entry is replaced with a special character (**0xE5**), marking it as deleted. The rest of the entry, including file size and starting cluster, **remains intact**.
* *Example* - If a user deletes a confidential document named "Report.doc," the directory entry is marked as deleted, but the content persists on the disk until overwritten, enabling forensic tools to recover the file.
## Fragmentation Challenge
* FAT is prone to file fragmentation, where data of a single file is scattered across non-contiguous clusters. When a file is deleted, the pointers that help link its clusters are also changed to zeros, which complicates data recovery and analysis efforts.
* *Example* - Recovering a fragmented video file from a FAT-formatted SD card may require reassembling multiple non-sequential data clusters.
## File Slack Space
* Due to fixed cluster sizes, small files or the final cluster of a file may not fully occupy the allocated space, leaving residual sectors known as slack space. This space can contain remnants of previously deleted files or other sensitive information.
* *Example* - A small text file occupying only part of a cluster may leave behind slack space containing fragments of an old email, potentially revealing additional evidence.
## Timestamp Artifacts
* **Limited timestamp resolution**: FAT records file creation, modification, and access times with limited accuracy, potentially hindering precise timeline analysis.
- **Timezone ambiguity**: FAT timestamps are stored in local time rather than UTC, which can cause discrepancies when moving drives between different time zones. Timestamps in FAT do not store timezone information, which can complicate correlating events across different systems.
- *Example* - A FAT-formatted device might reveal that a file was modified at "10:30 AM," but without timezone context, it may be challenging to determine the exact time of the event.
