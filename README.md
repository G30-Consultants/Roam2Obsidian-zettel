# Roam JSON To Zettel Notes

This is a forked repository from [renerocksai/rj2obs](https://github.com/renerocksai/rj2obs) with few more **additional features** and then forked again from GanguLabs/Roam2Obsidian:main. to be used as the core for converting Roam JSON to Zettel Notes:

* Generate HTML and Text Summary and Note bodies. 
___

Converts Roam JSON export to Zettel Notes.


Output is a regular set of Zettel Notes in a specified Kasten path with references maintained but also converted to Zettel links. 
### Features:

* Daily note format is changed to YYYY-MM-DD
* roam's block IDs are appended (only) to blocks actually referenced and converted to Zettel anchor links.
* Blockrefs, block mentions, block embeds are used to build the Reference side of the note, including embeds which are thumbnailed
* The Zettel schema is used as the default, including creation datetime and title.
* 
---
title:   
created: YYYY-MM-DD
---

```

* Top level roam blocks that don't contain children are not created as notes.

```

# Install
No need to install. But you need python3. Google is your friend. 

To install the required python packages:

```bash
pip install -r requirements.txt
```

# Usage:
```bash
python r2o.py my-roam-export.json
```

