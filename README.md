CourseraDownloader
==================

Simple set of scripts to deal with downloading Coursera courses, putting them into
a reasonable directory structure and then concatenating the videos by week into single
files.

### Usage

Usage: ./download-coursera [-hv] [-u username] [-p password] [-d output_dir] [-n skip_extensions] [-r reverse_section_order] [course_names...]

### Dependencies

- ffmpeg
-

### Configuration

To configure this script create a file at ~/.config/coursera_downloader.  It accepts
the following options:

- username
- password
- output_dir
- processed_output_dir
- courses
- skip_extensions
- reverse_order

An example file would look like:

```
username=my_user_name
password=my_password
output_dir=my_directory
processed_output_dir=my_processed_directory
courses=(course1 course2 course3)
skip_extensions="ppt,srt,pdf"
reverse_order=true
```
