# Odoo Project Management Application for Small and Medium Size businesses 

## Supported versions: Odoo 10/11

 This application module contains the basic templates for project management follow up and cost analysis.
It allows project managers to create and follow theirs projects and group them in programs, each projects beside the general attributes it contains the Risk & Issues and the resolution.

![Main Dashboard](https://res.cloudinary.com/t3-solutions-llc/image/upload/v1571152176/Capture_ikbh8t.jpg)

### Main entities:
* Project
* Program
* Risk
* Issues
* Project Type
* Project Managers
* Program Managers

### Additional features

* Document Management
* Kanban and Chart views.
* Custom project reports

For any changes and support feel free to contact me at: lyasine@3t-solutions.us


### Docker
The project is also available in docker hub, you could try it from :

```docker pull lyasine/dpms```

Then create the first PostgreSQL container and link it to the dpms container as the following:

```docker run --name dpmsdb -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo -e POSTGRES_DB=postgres -d postgres```

Then create the the dpms container:

```docker run --name dpms  --link dpmsdb:db -p 8069:8069 -d lyasine/dpms:latest```

Project chart report:

![Projects Report](https://res.cloudinary.com/t3-solutions-llc/image/upload/v1571152176/Capture3_nsxy3b.jpg)


