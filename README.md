# File Server in PHP
Serve the files in PHP so that you can Authenticate the USERS showing the content

## Usage

```sh
// Get the absolute path of the file. For Example: "C:/Users/Arif/myfile.ext", "/path/video.mp4" etc...
$path = "/path/file" ;

/*
Write all your athentication here, before the FileServer($path)->serve() is called
*/

$file = new FileServer($path);
//- serve the file. the header will be added for every particular file type.
$file->serve();
//exit();
```
