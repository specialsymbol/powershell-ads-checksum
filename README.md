# powershell-ads-checksum
Adds checksums to an alternate data stream of files using a powershell script

Seems to run fine. In fact, it does find all files and work as intended - the files I used for testing had one file that already had a valid MD5 alternate data stream. This was correctly ignored in the creation script and correctly verified in the checking script. So all my complaints about get-childitem not finding a file because of a more than three character extension are wrong - I just forgot it already had the MD5 stream.
