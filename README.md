# music-podcast-analyzer

Finds start and end ranges of music in podcast files (could be any audio files).

A common use case is enabling to generate chapter markers.


## Usage

```
$ ./analyze
Usage: analyze <audiofile>
```


### Example

```
$ ./analyze Bitar_till_Kaffet_024.mp3
Running: sox Bitar_till_Kaffet_024.mp3 -V1 --null remix 1,2 spectrogram -x 8016.873991 -y 1025 -l -m -r -o /var/folders/3g/ntlq0qcs0q344mdh08dg1dy40000gn/T/sox_XurDQU.png
Parsing spectrogram: /var/folders/3g/ntlq0qcs0q344mdh08dg1dy40000gn/T/sox_XurDQU.png
from [hh:mm:ss]      to [hh:mm:ss]  len [hh:mm:ss]  from [s]    to [s]  len [s]
    5:21                 8:01           2:40          321        481     160
   15:31                19:07           3:36          931       1147     216
   25:49                28:13           2:24         1549       1693     144
   36:35                40:23           3:48         2195       2423     228
   45:56                47:51           1:55         2756       2871     115
   53:30                57:44           4:14         3210       3464     254
 1:02:42              1:07:39           4:57         3762       4059     297
 1:18:19              1:21:00           2:41         4699       4860     161
 1:24:16              1:27:37           3:21         5056       5257     201
 1:37:16              1:38:33           1:17         5836       5913      77
 1:45:58              1:47:56           1:58         6358       6476     118
 1:54:08              1:56:59           2:51         6848       7019     171
 2:01:02              2:02:26           1:24         7262       7346      84
 2:11:02              2:13:36           2:34         7862       8016     154
