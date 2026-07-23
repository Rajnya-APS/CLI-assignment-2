# Question 1

# Commands Used

mkdir
cd
echo
cp
md5sum
chmod
cat

# Explanation

The script compares files using their MD5 checksum. If two files have the same checksum, they are considered duplicates. Unique files are copied to the backup directory, while duplicate files are skipped. A report summarizing processed, duplicated, and backed-up files is generated, and any errors are redirected to a separate file using `2>>`
