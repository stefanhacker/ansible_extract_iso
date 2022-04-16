An ansible role to exctract an folder. The Inbuilt iso function dont extract an folder




Description of Variables

path_to_iso: /tmp/myiso.iso
path_to_extract_dest: /tmp/extractediso/

#if you dont want extract the wohle iso, only a folder or file from, default empty
#extract_folder_and_files_from_iso: []
#an example
#extract_folder_and_files_from_iso:
 #- live/filesystem.squashfs
 #- casper/*

#overwrtie switch (default it skipped existing files folders)
#Switch Description
# -aoa  Overwrite All existing files without prompt.
# -aos  Skip extracting of existing files.
# -aou  aUto rename extracting file (for example, name.txt will be renamed to name_1.txt)
# -aot  auto rename existing file (for example, name.txt will be renamed to name_1.txt)
overwrite: -aos
#extracted with complete folder structure.
fullpath_paremeter: x