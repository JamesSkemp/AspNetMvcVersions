ASP.NET MVC Versions
=================

This is a collection of out-of-the-box ASP.NET MVC project versions.

The ultimate goal is to determine how things have actually changed between versions, to both ease the upgrade path and determine how to revert back, if necessary.


Temporary Notes
=====

Visual Studio 2012 and Visual Studio 2012 Update 1 have no real changes to the ASP.NET MVC 3 projects, with the exception of the following code, added immediately before the system.web sessionState element in the root Web.config:

    <!--
            If you are deploying to a cloud environment that has multiple web server instances,
            you should change session state mode from "InProc" to "Custom". In addition,
            change the connection string named "DefaultConnection" to connect to an instance
            of SQL Server (including SQL Azure and SQL  Compact) instead of to SQL Server Express.
      -->
