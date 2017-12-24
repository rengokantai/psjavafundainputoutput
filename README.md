# psjavafundainputoutput

## 3. Reading Characters
### 8 Creating Readers for Disk and in-memory operations
1) class for certain type of input
- Disk: FileReader
- In-memory: CharArrayReader, StringReader

2) class that add behavior to reader
- BufferedReader
- LineNumberReader
- PushbackReader

```
Filereader filereader = new FileReader(file)
LinuNumberReader/BufferedReader rd = new LineNumberReader(filereader);
```
```LineNumberReader``` extends ```BufferedReader```

### Java 7 Patterns to Create Readers with Specific Charsets
```
Path path = Paths.get("files/data.txt");
BufferedReader reader2 = Files.newBufferedReader(path, StandardCharsets.ISO_8859_1);
```
