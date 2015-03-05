Cloudwick Labs Synthetic Data Generators
----------------------------------------

These data generators mocks several real-life situations. Purpose built for research and development of several big data use cases.

| Generator | Description | Schema | Scope |
| :---: | --- | --- | --- |
| **log** | mocks the logs generated by apache [httpd](http://httpd.apache.org/) | [Log Schema](https://github.com/cloudwicklabs/generator/wiki/Log-Schema) | 1. Real time data ingestion (using Flume & MapReduce)<br> 2. Real time analytics (using Storm and kafka)<br> 3. Click stream analytics<br> 4. NoSql |
| **odvs** | mocks the data generated by a real life on-demand video service provider like netflix, hulu & amazon prime | [ODVS Schema](https://github.com/cloudwicklabs/generator/wiki/ODVS-Schema) | 1. NoSql<br> 2. Analytics using MapReduce/Hive |
| **osge** | mocks the data generated by a online social gaming entertainment provider like second life, imvu, onverse... | [OSGE Schema](https://github.com/cloudwicklabs/generator/wiki/OSGE-Schema) | 1. NoSql<br> 2. Analytics using MapReduce/Hive |

###Build from source
This project requires [sbt](http://www.scala-sbt.org/), installation instructions found [here](http://www.scala-sbt.org/release/docs/Getting-Started/Setup.html)

Once, sbt is installed use the `assembly` sbt task from the project path to build the jar with dependencies

```
git clone https://github.com/cloudwicklabs/generator.git
cd generator
sbt assembly
```

###Running the generator
Use the built in shell wrapper to fire up the generator

```
bin/generator --help
```

###Using individual generators

All the data generators have a driver command line interface, following links show basic examples

* [Log generator](https://github.com/cloudwicklabs/generator/wiki/Log-Generator-Driver)
* [ODVS generator](https://github.com/cloudwicklabs/generator/wiki/ODVS-Generator-Driver)
* [OSGE generator](https://github.com/cloudwicklabs/generator/wiki/OSGE-Generator-Driver)

###Feedback
For more generators, your specific use-cases or to leave feedback contact [support](mailto:support@cloudwick.com)

###License and Authors

**Authors**: [Ashrith](https://github.com/ashrithr)

Apache 2.0. Please see `LICENSE.txt`. All contents copyright (c) 2013, Cloudwick Labs.
