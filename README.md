# DownloadX

Content download CLI tools

## Installation
```sh
pip install downloadx
```

## Using downloadx CLI
### Get help
```sh
downloadx -h
```

### Download YouTube content
#### Get help
```sh
downloadx youtube -h
```

#### Download single url
```sh
downloadx youtube --url https://www.youtube.com/watch?v=aWYgotleA2w
```

#### Download multiple YouTube url
create any file to store the url of the content to be downloaded.
for example, create a **urls.txt** file 
```txt
https://www.youtube.com/watch?v=aWYgotleA2w
https://www.youtube.com/watch?v=26JMKOsc8c8&t=254s
https://www.youtube.com/watch?v=Wqr-uZInkQ0
https://youtu.be/Nq4Mh_jTubA
```

run the download command by defining the `--url-file` argument
```sh
downloadx youtube --url-file urls.txt
```

#### Download audio only
By default download x will download youtube video content. if you want to download audio only, you can add the `--audio-only` argument
```sh
downloadx youtube --url https://www.youtube.com/watch?v=aWYgotleA2w --audio-only
```

#### Download file directory
By default, downloaded files will be stored in the **./outputs** directory, if you want to change the output directory you can add the `--output` argument as follows:
```sh
downloadx youtube --url-file urls.txt --output /mydir/location
```

