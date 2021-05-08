# PostgreSQL Parameter Tuning CheatSheet
<div style="text-align: justify">
PostgreSQL is a free and open-source relational database management engine. Often ranked among the top database choice (with or without financial considerations), has also been referred to as the worlds best database with respect to performance, transperant security, multiversion concurrancy, stability, licensing, documentation by many.
</div>

## Criterias for achieving a highly performant PostfreSQL database
- Good data model, database design, & data organization
- Performant hardware, disk layout, & **file system configuration**
- Tuning the database **configuration parameters** in accordance with the above

# How to use this CheatSheet?
<div style="text-align: justify">

PostgreSQL has over 200 coniguration parameters. These parameters can be tuned by editing the *postgresql.conf* file which is usually located at */var/lib/pgsql/data/postgresql.conf*. Configuring the parameters is necessary as the default parameters are not tuned for the specific hardware where the database will functional. This CheatSheet provides a quick overview of the **most** critical set of parameters which should be looked at and tuned for performance. Along with 
the parameters present in the PostfreSQL configuration file (Autovacuum, Memory, Asynchronous behaviour, Write-Ahead log and logging), the CheatSheet also lists some Kernel setting parameters, which also affects the PostgreSQL performance and should **definetely** be looked at. The CheatSheet thus provides a quick overview along with the parameter name, their default values, a small description and the **recommended setting**. The recommended parameter values **should be used meticulously** with peformance benchmarking.
  </div>

# References and Benchmarking Extensions/Tools
- https://postgresqlco.nf/doc/en/param/
- https://www.2ndquadrant.com/en/
- https://www.postgresql.org/docs/10/pgbench.html
- https://www.postgresql.org/docs/9.4/pgstatstatements.html
- https://github.com/darold/pgbadger

