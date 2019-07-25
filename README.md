
codec
====

Golang aac decoder.

AAC decoding example:

```go
var header []byte
var pkts [][]byte

dec, _ := codec.NewAACDecoder(header)
for _, p := range pkts {
	sample, err := dec.Decode(p)
}
```

License
----

All code is under WTFPL. You can use it for everything as you want :)
