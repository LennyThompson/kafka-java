# Java Model Schema

Simple kava project that simply generates the java source from the protobuf model schema and builds a jar library.

Not the best way to do this, but it works. Well sort of.

There is some problem with the generator so that if the java has already been generated the build will fail...

Almost entirely defined in the *pom.xml* - see *protoc-jar-maven-plugin*

Note the generated java is strongly dependent on the protoc plugin version, and the protoc compiler version installed. Both the producer and consumer of data in the schema **must** be built with a compatible version, which more or less means the same version.