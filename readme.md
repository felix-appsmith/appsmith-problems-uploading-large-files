# Test details
1. What does this test prove?
    - This test seeks to test the upload of files of different sizes to determine what causes the upload of large files to fail.
  
2. Why are these tests being done?
    - These tests are being carried out because this [user](https://app.frontapp.com/open/msg_1fv1vkb0) reported the problem and other users have previously presented similar problems.
3. How the tests are carried out
   - A simple file upload system was created with the ability to upload multiple files at the same time or individually, a Postgres database was used.
   - You can do your own tests using this [app](https://app.appsmith.com/app/filesuploaderror/page1-636914a6b7d12f577aa56521) on Appsmith support account
   - You can create your Postgres database using this [guide](https://github.com/felix-appsmith/appsmith-quick-datasources#-postgresql)
   - connect the created database to the application
  
## Test 1 Specifications

### File Types
    - MP4
    
### Video file sizes
    - 3.9mb
    - 13.1mb
    - 58.3mb

### Computer specification
    - SO : Pop Os
    - Ram: 16gb
    - CPU:Rayzen 5 5600G
    - Main disk: HDD 500gb
    - Network speed: 200mb / 200mb

### Browser
    - Chrome
    - FireFox


## Test 1 results

### Chrome

1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`
4. 3 All files at the same time `failed`

### Firefox

1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`
4. 3 All files at the same time `failed`

### Notes
1. The upload fails but shows no errors.
2. The result in the two browsers that was tested is the same and has the same behavior of the video


## Test 2 Specifications

### Video file sizes
     - 3.9mb
     - 13.1mb
     - 58.3mb

### Computer specification
    - SO : Windows10
    - Ram: 48gb
    - CPU:Rayzen 9 5900X
    - Main disk: SSD 1tb 
    - Network speed: 200mb / 200mb

### Browser
    - Chrome
    - FireFox
    - Microsoft edge

## Test 2 results

### Chrome
1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`
4. All files at the same time `failed`

### Firefox
1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`
4. All files at the same time `failed`

### Microsoft Edge

1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`
4. All files at the same time `failed`

# Notes
1. The upload fails but shows no errors.
2. The results were the same in both Tests, that is why only a video is shown because the behavior was the same.


## Test 3 Amazon S3

### File Types
    - MP4
    
### Video file sizes
    - 3.9mb
    - 13.1mb
    - 58.3mb

### Computer specification
    - SO : Pop Os
    - Ram: 16gb
    - CPU:Rayzen 5 5600G
    - Main disk: HDD 500gb
    - Network speed: 200mb / 200mb

### Browser
    - Chrome
    - FireFox

## Test 3 results

### Chrome
1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`

### Firefox
1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `failed`

# Video of the tests carried out

## Test 4 Download local files

### File Types
    - MP4
    
### Video file sizes
    - 3.9mb
    - 13.1mb
    - 58.3mb

### Computer specification
    - SO : Pop Os
    - Ram: 16gb
    - CPU:Rayzen 5 5600G
    - Main disk: HDD 500gb
    - Network speed: 200mb / 200mb

### Browser
    - Chrome
    - FireFox

## Test 4 results

### Chrome
1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `Success`

### Firefox
1. 3.9 MB file `Success`
2. 13.1 MB file `Success`
3. 58.3 MB file `Success`

`Note: Although all downloads are successful, files that are treated as blobs do not work. Example without a file that is a video weighing 23MB it will be downloaded and will weigh 56 Bytes and will not be able to be played`

https://user-images.githubusercontent.com/114161539/200386904-8efa1512-f162-4394-bea0-32ab3ccbb284.mp4

