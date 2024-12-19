# ISBN Explorer
ISBNs torrent source: 
- https://annas-archive.org/torrents/aa_derived_mirror_metadata
- https://annas-archive.li/db/aarecord/md5:8336332bf5877e3adbfb60ac70720cd5.json
- Standard Anna's Archive release format design: https://annas-archive.li/blog/annas-archive-containersb.html
- ISBN metadata dump format: https://software.annas-archive.li/AnnaArchivist/annas-archive/-/blob/369f1ae1074d8545eaeaf217ad690e505ef1aad1/allthethings/cli/views.py?page=2#L1244-1319

## Minimum requirements
- Fork this repo, and edit this blog post HTML (no other backends besides our Flask backend are allowed).
- Make the picture above smoothly zoomable, so you can zoom all the way to individual ISBNs. 
  - Clicking ISBNs should take you to a metadata page or search on Anna’s Archive.
- You must still be able to switch between all different datasets.
- Country ranges and publisher ranges should be highlighted on hover 
  - (you can use e.g. data4info.py in isbnlib for country info, and our “isbngrp” scrape for publishers).
- It must work well on desktop and mobile.

## Front-end ISBN Data representation


## Questions
- Does all_isbns refer to all of the currently registered ISBNs across all the available datasets?
  - Are any of the individual ISBN datasets comprehensive (e.g. isbndb?)
  - Either way, the entire set should be taken as the union of all of the datasets. We can diff individual datasets against the union anyway.

