# Serialization and Streams

```java
try (
  FileOutputStream fos = new FileOutputStream("treets.ser");
  ObjectOutputStream fos = new ObjectOutputStream(fos);
) {
  oos.writeObject(treets);
} catch (IOException ioe) {
  System.out.println("Problem saving treets");
  ioe.printStackTrace();
}
```

## Serialisation Versioning
Use `serialver`, eg:

```bash
serialver com.treehouse.Treet
```
