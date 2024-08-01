
<br>

<p style="text-align: center;font-size:120%">*A very very brief overview of the <tt>openapx</tt> project ... more details to come.*</p>

<br>

<tt>openapx</tt> is an Open Source project to create and maintain an open and scalable architecture for analysis, programming and compute for the Life Science and other regulated industries. Rather than create one big silo, the capabilities of <tt>openapx</tt> is viewed as a set of micro-services that combined provide the necessary resources.

The project consists of a set of containers for the compute layer as well as tools, utilities, dashboards, etc. to interact with and manage the environments, work and effort.

<br>

### Compute containers
The <tt>openapx</tt> project currently develops and maintains a set of baseline containers for R across multiple operating systems that will be extended to other languages as well, Python being one such example. 

The container architecture and provenance is designed to simplify compliance processes and documentation, e.g. tested and validated once and use everywhere.

The current R containers under development are 

- [rbin](https://github.com/openapx/docker-rbin) is a binary complete container hosting multiple versions of R (currently the last patch for minor releases that can be built on the same tool chain) 
- [rbatch](https://github.com/openapx/docker-rbatch) is a container extending `openapx/rbin` with core R packages, currently 160+ and growing
- [rworkbench](https://github.com/openapx/docker-rworkbench) is essentially the `openapx/rbatch` container with Posit/R-Studio Workbench (Open Source license)

There are other containers already planned for R

- rwapp – a container extending `openapx/rbatch` for use with R Web applications like {shiny}
- rapi – a container extending `openapx/rbatch` for use with R APIs written with {plumber}
- rminimal – a minimized container with only the latest released R version
- rdevel – a container extending `openapx/rminimal` for use in R package build and testing processes
- rminwapp - a container extending `openapx/rminimal` for use with R Web applications like {shiny}
- rminapi – a container extending `openapx/rminimal` for use with R APIs written with {plumber}
- rdbench – a container extending `openapx/rworkbench` or `openapx/rminimal` for use in R package and application development

<br>

### Compliance
The <tt>openapx</tt> deliverables will be documented and tested to support Life Science GxP-level validation and validation requirements for other regulated industries. The formal validation is of course still the responsibility of each individual organization that uses the <tt>openapx</tt> deliverables, our aim is just to provide some standardization and save you a lot of effort.
