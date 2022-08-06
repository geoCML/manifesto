# geoCML Manifesto 

geoCML is a deployment pattern for Containerized Multi-paradigm Lightweight GISystems running locally or in the cloud. geoCML deployments are built with Docker using a single base image. This image installs the following software to the container:

    • QGIS 
    • QGIS Server
    • Apache Web Server
    • PostgreSQL
    • Redis
    • … and any additional software you need for your deployment

When users build their container from the geoCML base image, their container is automatically configured with a PostgreSQL database (with Redis integration), QGIS Server API, and a new QGIS project. Each geoCML deployment is intended to have only one GISystem; users who want to have multiple GISystems will need multiple geoCML deployments. An entire GIS deployment can be completed in a few minutes. 

geoCML deployments can be run locally or on a hosted web server. When a geoCML deployment is hosted, the URL and description for that GISystem are posted to the DRGON (Distributed Registry of GISystem Over a Network). The DRGON is a single webpage containing information on all geoCML deployments, allowing users to quickly find interesting GISystems. Users can also use the DRGON to fork a GISystem in order to create their own GISystem using preexisting data.

Using Kasm, users can sign into their GISystem and interface with it via an immutable desktop interface. Users may also interact with their GISystem via QGIS Server for automated tasks. geoCML deployments can be made public, or can be protected via a password. Password protected deployments cannot be forked via the DRGON unless the user forking the system knows the correct password. geoCML deployments also support real-time collaboration with multiple concurrent users. 

geoCML, including all of the repositories under github.com/geoCML, is open-source and community owned. As a community, we all must share a common goal of developing geoCML as GIS for good. GISystems provide a tremendous amount of potential for good (supporting conservation efforts, combating the climate crisis, academic research, highlighting and enacting change for policial and social issues, etc), though history has unfortunately proved that they can also be used for evil (racial redlining, developing natural gas/oil pipeline through indigenous protected lands, supporting war efforts abroad, etc). While geoCML software comes without warranty, we all must work together to encourage the ethical use of geospatial technology so that we may all may prosper on this planet.
