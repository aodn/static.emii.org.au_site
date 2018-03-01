
### Message Of The Day - usage

`index.txt` is the target of the portal config item `motdUrl`

```
portal {
    motdUrl = "https://s3-ap-southeast-2.amazonaws.com/static.emii.org.au/portalMotd/index.txt"
    .....
```
    
- If `index.txt` exists and has at least one line in it, it will be used by the portal to show a 'message of the day'. 

- The file should have two plain text lines:
   -  first line is the title
   -  Second line is the message body. 

- One line only will have the default title of "_Notice_" and the supplied line will show as body text.
- The portal will ignore an empty file or missing file.
- The portal should address `index.txt` via the direct link https://s3-ap-southeast-2.amazonaws.com/static.emii.org.au/portalMotd/index.txt avoiding caching.
