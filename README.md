Public Notifications Data Format project
====

This is a project by the San Francisco Mayor's Office of Civic Innovation to establish best practices for public notifications by City departments and to standardize messaging. 

The Public Notifications Data Format (PNDF) will be a data layer produced from existing data held by city departments, capable of accommodating the full spectrum of public notices, including filming permits, road closures, tree removals and license applications. 

SFMOCI intends to pilot the use of the PNDF with platform partners in Fall 2014, to enable members of the public to browse and search notifications, and to subscribe for updates on given topics in their chosen geographic area of interest. 

This repo contains notification.txt, a schema that lists the proposed fields to be used in public notifications, and notification_types.txt, an in-progress typology of notifications produced by City departments. Both are at a draft stage; comments and additions are encouraged.


Notes on the PNDF format
========================

project_id // Generated by the platform. Format TBD, could be [Dept Code / Year / Month / ID] e.g. 011306XXX

notification_type // TBD: Pending the completion of notification_types.txt 

project_ref // The department’s internal reference number

project_geometry // KML geometry in the format <LineString><coordinates>lat,long lat,long</coordinates>

project_status // A free text entry that describes the current status of the project, e.g. (Planning, Consultation, Construction). The entries given will differ between departments, but it is valuable since users can subscribe to be notified of a change in this field.

project_siblings
project_ref of related permits, so that the platform can associate them