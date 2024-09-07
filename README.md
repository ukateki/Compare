# Compare
Compare files from a local directory or a remote URL.

This program allows you to compare two files (local or from a URL) by sampling random chunks from each file and generating checksums to determine if the files are identical. The program uses curl for fetching chunks from URLs and dd for reading chunks from local files. It supports both MD5 and SHA1 checksums for verification.

## Instructions for Use
### Install on macOS
- Open Terminal and execute the following command:
```
sudo mkdir -p /usr/local/bin && sudo curl -o /usr/local/bin/compare https://raw.githubusercontent.com/ukateki/Compare/main/compare && sudo chmod +x /usr/local/bin/compare
```
[What is terminal?](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac)


You may be required to enter a password. This password is your login password and is secure.

### Usage
- Open Terminal and execute the following command:
```
compare <file1> <file2>
```
- `<file1>`: Path or URL of the first file to compare.
- `<file2>`: Path or URL of the second file to compare.

### Update
- Execute this command once more.
```
sudo mkdir -p /usr/local/bin && sudo curl -o /usr/local/bin/compare https://raw.githubusercontent.com/ukateki/Compare/main/compare && sudo chmod +x /usr/local/bin/compare
```
You may be required to enter a password. This password is your login password and is secure.

### Remove
- Open Terminal and execute the following command:
```
sudo rm /usr/local/bin/compare
```
You may be required to enter a password. This password is your login password and is secure.

### Notes
- The program samples 50 random 1 KB chunks from each file for comparison.
- If the file sizes differ, the program will immediately report a difference.
- The program requires curl and dd commands to handle URLs and local files.
- Ensure the provided files or URLs are accessible.

### Discuss
We have a Telegram Group for discussion: [Digital Divinity Chat](https://t.me/Digital_Divinity_Chat)
