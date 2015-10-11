## sample_square

the sample square maps wav samples to a two dimensional field based on PCA using musical analysis from spotify. 

users can play clips by clicking on various spots of the heat map

to set up, download the wav files into /sounds with the following code

```python
def download(id_num):
    s3_key = wavs[i][1]['s3_key'][:-4] + '.mp3'
    ID = wavs[i][0]['original_id'] + '.mp3'
    print(start + s3_key)
    urllib.request.urlretrieve(start + s3_key, location + ID)
    print(str(n) + ' done!')
    n += 1
```

to run, execute `gui.py`