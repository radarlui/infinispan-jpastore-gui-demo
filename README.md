Infinispan GUI Demo on JPA Cache Store
-------------------

Infinispan comes with a GUI demo, to visually demonstrate state being moved around a cluster.

The demo is packaged in the infinispan-<version>-all.ZIP and infinispan-<version>-bin.ZIP distributions.

This JPA Cache Store demo is modified base on the Infinispan GUI Demo to demonstrate preloading and persistence using JPA Cache Store.

Before running the demo, please launch a MySQL server and then modify the connection parameter accordingly in src/main/resources/META-INF/persistence.xml

The demo can be launched using the runGuiDemo.sh script from the src/main/release/bin with the default configuration file jpa-cache-config.xml. 

Note that the configuration file used by the demo can be changed by modifying runGuiDemo.sh to pass in

   file:///path/to/config.xml

to your JVM.  This allows you to try out and visualize different configurations.  If you are running the demo in a
clustered mode, it would make sense to launch several instances of the demo and watch data move around across different
instances.

