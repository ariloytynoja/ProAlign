# ProAlign

This is the legacy code for the ProAlign multiple sequence alignment method.

The source code (proalign_0.5a0.tar.gz) and the compiled jar-file (proalign.jar) can be found in the directory [files](files/).

The method is described in the [original article](https://academic.oup.com/bioinformatics/article-abstract/19/12/1505/257958) and in the document [ProAlign.pdf](files/ProAlign.pdf).

### Usage

```
java -jar proalign_0.5a0.jar
```


### Compilation

```
tar xzf proalign_0.5a0.tar.gz
javac -Xlint:deprecation -Xlint:unchecked -d . *java
mkdir META-INF
cat > META-INF/MANIFEST.MF << EOF
Main-Class: proalign.ProAlign
EOF
jar cmf META-INF/MANIFEST.MF proalign.jar proalign/*class
```

This software is no more supported.