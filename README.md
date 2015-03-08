#faketag - the android based emulator of nfc tags 

Goal of this project is to create a simple android based emulator for nfc tags.
Processing of APDU's is based on a simple json file.

##JSON file format

This emulator is processing apdu commands based on simple JSON files. Use the following format:

```json
[
	{"request":"80CA9F7F00","response":"6800"},
  	{"request":"12345","respone":"12345"}
]
```

So if you sniff sessions from real world nfc-tags you can generate a json-file like the above and
your able to emulate this nfc tag. At the moment only statically tags without any random data are 
supported.
