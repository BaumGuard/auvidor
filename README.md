# auvidur
Bash tool for summing up durations of audio and video files<br/>
**Linux only!**

## Dependencies
- `exiftool`

## Installation
Clone the repository to your home directory:
```
git clone https://www.github.com/BaumGuard/auvidur
```
Enter the folder:
```
cd auvidur
```
Make the script executable:
```
chmod 777 auvidur
```

To start `auvidur` from anywhere, just copy it to `/usr/bin`:
```
sudo scp auvidur /usr/bin
```
## Usage
If you haven't copied `auvidur` to `/usr/bin` you have no navigate to the folder of `auvidur` and start it from there:<br/>
```
./auvidur
```
or
```
bash auvidur
```
Otherways just write "auvidur".<br/>
<br/>
Enter the file names or file paths after "auvidur". You can also select a bunch of files in your file manager, copy them and paste them after "auvidur". For example like this:
```
auvidur /path/to/file1.wav /path/to/file2.mp3 /path/to/file3.ogg
```

Now hit Enter and you should see the summed-up duration on the bottom.<br/>
Depending on how many files paths you have entered it might take a while until you see the result.
## Troubleshooting
There are cases in which you might be faced with this error:<br/>
`expr: Syntax error: missing argument after "+"`<br/>
This can happen if you have entered files that can not be classified as audio or video. Normally they shouldn't affect the total duration.
