# powershell-ads-checksum
Adds checksums to an alternate data stream of files using a powershell script

Seems to run fine. In fact, it does find all files and work as intended - the files I used for testing had one file that already had a valid MD5 alternate data stream. This was correctly ignored in the creation script and correctly verified in the checking script. So all my complaints about get-childitem not finding a file because of a more than three character extension are wrong - I just forgot it already had the MD5 stream.

ToDo:
- Create functions to streamline the code
- Always check files first and create a file with the file info (checksum, CreationTime, LastWriteTime, Length (Filesize)) for files that already have a MD5 stream

For the future: create a standalone file that can be executed in a directory and uses its location. Maybe even add the option to select various Hash functions and if it should be recursive
