```
1  sudo apt update
2  sudo apt search exiv2
3  sudo apt install exiv2
4  exiv2 6afe7186-ea2f-4a5c-ac68-0186a332454d.jpg 
5  exiv2 7d74b3c7-f20d-4e2a-9465-dbefa051bd2f.jpg 
6  exiv2 IMG_6800.HEIC 
7  apt search exif
8  sudo apt install exifprobe
9  exifprobe 6afe7186-ea2f-4a5c-ac68-0186a332454d.jpg 
10  exifprobe IMG_6800.HEIC 
11  sudo apt install exiftool
12  exiftool IMG_6800.HEIC 
13  exiftool 6afe7186-ea2f-4a5c-ac68-0186a332454d.jpg 
14  exiftool 5883997061584634559.jpg 
15  exiftool --help
16  man exiftool 
17  exiftool --geotag IMG_6800.HEIC 
18  exiftool  IMG_6800.HEIC 
19  exiftool -geotag=trac.kml ./*.HEIC
20  hexdump -C 5883997061584634559.jpg > 5883997061584634559.jpg.hex
21  awk -F' ' '{print $2$3$4$5$6$7$8$9}' 5883997061584634559.jpg.hex | xxd -r -p > p.jpg
22  xxd 5883997061584634559.jpg
23  xxd 5883997061584634559.jpg > 5883997061584634559.jpg.xxd
24  awk -F' ' '{print $2$3$4$5$6$7$8$9}' 5883997061584634559.jpg.xxd | xxd -r -p > p.jpg
25  strings 5883997061584634559.jpg
26  strings 5883997061584634559.jpg > 5883997061584634559.jpg.strings
27  xxd blank.jpg > blank.jpg.xxd
28  xxd red.jpg > red.jpg.xxd
29  awk -F' ' '{print $2$3$4$5$6$7$8$9}' blank.jpg\ copy.xxd | xxd -r -p > p.jpg
30  xxd foto.jpg > foto.jpg.xxd
31  xxd foto-marker.jpg > foto-marker.jpg.xxd
32  cp foto.jpg.xxd foto.jpg.xxd-bis
33  awk -F' ' '{print $2$3$4$5$6$7$8$9}' foto.jpg.xxd-bis | xxd -r -p > p.jpg
34  history 
35  history > README.md
```

https://starkeblog.com/hexdump/binary/linux/2021/08/27/hexdump-to-binary.html

https://gist.github.com/leommoore/f9e57ba2aa4bf197ebc5?permalink_comment_id=3860213


The leftmost column is the hexadecimal displacement (or address) for the values of the following columns. Each row displays 16 bytes.

A hex file uses 2 hex digit characters to represent a single byte, plus the record overhead.

```
Hex	Char
00	NUL
01	SOH
02	STX
03	ETX
04	EOT
05	ENQ
06	ACK
07	BEL
08	BS
09	HT
0A	LF
0B	VT
0C	FF
0D	CR
0E	SO
0F	SI
10	DLE
11	DC1
12	DC2
13	DC3
14	DC4
15	NAK
16	SYN
17	ETB
18	CAN
19	EM
1A	SUB
1B	ESC
1C	FS
1D	GS
1E	RS
1F	US
20	space
21	!
22	"
23	#
24	$
25	%
26	&
27	'
28	(
29	)
2A	*
2B	+
2C	,
2D	-
2E	.
2F	/
30	0
31	1
32	2
33	3
34	4
35	5
36	6
37	7
38	8
39	9
3A	:
3B	;
3C	<
3D	=
3E	>
3F	?
40	@
41	A
42	B
43	C
44	D
45	E
46	F
47	G
48	H
49	I
4A	J
4B	K
4C	L
4D	M
4E	N
4F	O
50	P
51	Q
52	R
53	S
54	T
55	U
56	V
57	W
58	X
59	Y
5A	Z
5B	[
5C	\
5D	]
5E	^
5F	_
60	`
61	a
62	b
63	c
64	d
65	e
66	f
67	g
68	h
69	i
6A	j
6B	k
6C	l
6D	m
6E	n
6F	o
70	p
71	q
72	r
73	s
74	t
75	u
76	v
77	w
78	x
79	y
7A	z
7B	{
7C	|
7D	}
7E	~
7F	DEL
```
